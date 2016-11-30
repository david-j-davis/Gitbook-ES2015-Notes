#Destructuring
Destructuring lets you break apart an array or object into variables.

###Destructuring Objects
{% tonic %}
let toybox = { item1: 'car', item2: 'ball', item3: 'frisbee' };

let {item1, item2} = toybox;

console.log(item1);
{% endtonic %}

###Destructuring Arrays
{% tonic %}
let widgets = ['widget1', 'widget2', 'widget3', 'widget4', 'widget5'];

let [a,b,c, ...d] = widgets;

console.log(a);
{% endtonic %}

###Destructuring Nested Objects
{% tonic %}
let parentObject = {
  title: 'Super Important',
  childObject: {
    title: 'Equally Important'
  }
}

let { title, childObject: { title: childTitle } } = parentObject

console.log(childTitle);
{% endtonic %}
###Destructuring Default Functions
{% tonic %}
function getData({ url, method = 'post' } = {}, callback) {
  callback(url, method);
}

getData({ url: 'myposturl.com' }, function (url, method) {
  console.log(url, method);
});

getData({ url: 'myputurl.com', method: 'put' }, function (url, method) {
 console.log(url, method);
});
{% endtonic %}
