#For Of Loop
A new way to loop over items in an iterable like String, Array, Set, and Map
      let teachers = [
          { name: 'Ken', comments: 'Amazing', rating: 4 },
          { name: 'James', comments: 'Astounding', rating: 3 },
          { name: 'Dave', comments: 'Astonishing', rating: 3 },
          { name: 'John', comments: 'Accelerating', rating: 2 },
          { name: 'Andrew', comments: 'Arm-chair-ing', rating: 3 },
          { name: 'Elizabeth', comments: 'Accepting', rating: 5 },
          { name: 'Nick', comments: 'Automating', rating: 6 },
          { name: 'Sarah', comments: 'Amplifying', rating: 7 },
          { name: 'Alena', comments: 'Appending', rating: 8 }
      ];

###In ES5 we used the forEach loop to iterate over data, but every item is looped over
      teachers.forEach(teacher => {
        if (teacher.name === 'Nick') {
          console.log(teacher.rating);
        }
      });
###In ES6, the for of loop allows the loop it exit once the match is reached
      for (let teacher of teachers) {
        console.log(teacher.name);
        if (teacher.name === 'Nick') {
          console.log(teacher.rating);
        }
      }
###Live Example
{% tonic %}
for (let teacher of teachers) {
  console.log(teacher.name);
  if (teacher.name === 'Nick') {
    console.log(teacher.rating);
    break;
  }
}
{% endtonic %}
