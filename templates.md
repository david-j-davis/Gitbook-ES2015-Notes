#Template Strings
Concatenating strings in JavaScript has lead to a lot of confusion. With Template Strings we can safely construct strings with ease.


      const student = { name: 'James', followerCount: 34 };

      let tableHtml = `
        <table class="table">
          <thead>
            <tr>
              <td>Name</td>
              <td>Followers</td>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>${student.name}</td>
              <td>${student.followerCount}</td>
            </tr>
          </tbody>
        </table>`;

        console.log(tableHtml);

####Live Example
{% tonic %}
const student = { name: 'James', followerCount: 34 };

let tableHtml = `
  <table class="table">
    <thead>
      <tr>
        <td>Name</td>
        <td>Followers</td>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>${student.name}</td>
        <td></td>
      </tr>
    </tbody>
  </table>`;

console.log(tableHtml);
{% endtonic %}
