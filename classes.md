#Classes
---
    'use strict';

    class Person {
      constructor(name) {
        this.name = name;
      }
      sayHello() {
        console.log("hello from ", this.name);
      }
    }

    var sarath = new Person('Sarath');

    sarath.sayHello();

{% tonic %}
class Person {
constructor(name) {
  this.name = name;
}
sayHello() {
  console.log("hello from ", this.name);
}
}

var sarath = new Person('Sarath');

sarath.sayHello();
{% endtonic %}
