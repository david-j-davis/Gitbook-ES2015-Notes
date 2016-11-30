#Rest Parameters
Rest parameters let you specify an unknown number of parameters.

      function myFunction(name, ...params) {
      console.log(name, params);
      }

      myFunction('Andrew', 1, 2, 3);
####Live Example
{% tonic %}
function myFunction(name, ...params) {
console.log(name, params);
}

myFunction('Andrew', 1, 2, 3);
{% endtonic %}

#Spread Operators
The spread operator lets you specify an unknown number of array properties. In this video we’ll demonstrate how this is helpful.

      const originalFlavors = ['Chocolate', 'Vanilla'];

      const newFlavors = ['Strawberry', 'Mint Chocolate Chip'];

      const inventory = ['Rocky Road', ...originalFlavors, 'Neopolitan', ...newFlavors];

      console.log(inventory);
####Live Example
{% tonic %}
const originalFlavors = ['Chocolate', 'Vanilla'];

const newFlavors = ['Strawberry', 'Mint Chocolate Chip'];

const inventory = ['Rocky Road', ...originalFlavors, 'Neopolitan', ...newFlavors];

console.log(inventory);
{% endtonic %}
