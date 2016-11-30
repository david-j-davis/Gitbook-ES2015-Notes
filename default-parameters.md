#Default Parameters
We’re able to set default values for function parameters like every other programming language. 

#####ES5 default params method
      function greet(name, timeOfDay) {
        name = name || 'Guil';
        timeOfDay = timeOfDay || 'Day';
        console.log(`Good ${timeOfDay}, ${name}!`);
      }
      greet();
#####ES6 default params method
      function greet(name = 'Guil', timeOfDay = 'Day') {
        console.log(`Good ${timeOfDay}, ${name}!`);
      }
      greet();
####Live Example
{% tonic %}
function greet(name = 'Guil', timeOfDay = 'Day') {
  console.log(`Good ${timeOfDay}, ${name}!`);
}
greet(undefined, 'Afternoon');
{% endtonic %}
