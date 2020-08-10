# Daily read 07

## Domain Modeling
### Summary
Domain modeling is the process of creating a conceptual model for a specific problem.

- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the `this` variable within methods so you can access the object's properties and methods from inside.
```
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}
var parkourFail = new EpicFailVideo(7,false);
var corgiFail = new EpicFailVideo(4,true);

console.log(parkourFail);
console.log(corgiFail);
```

## Tables
- Basic structure
```
<table>
<tr>
<td>15<td>
<td>15<td>
<td>30<td>
</tr>
<tr>
<td>45<td>
<td>60<td>
<td>30<td>
</tr>
</table>
```
- the `<table>` element is used to add tables to a web page.
- A table is drawn out row by row. Each row is created with the `<tr>` element.
- Inside each row there are a number of cells represented by the `<td>` or `<th>` if it's a header
- You can make cells of a table span more than one row or column using the rowspan and colspan attributes
- For long table you can split the table into a `<thead>`, `<tbody>`, and `<tfoot>`


## Functions, Methods, and Objects
- Functions allow you to group a set of related statements together that represent a single task.
- Functions can take parameters and may return a value
- An object is a series of variables and functions that represent something from the world around you
- In an object, variables are known as properties of the object; functions are known as methods of the object
- Web browser implement objects that represent both the browser window and the document loaded into the browser window
- JavaScript also has several built-in objects such as String, Number, Math, Date
- Arrays and objects can be used to create complex data sets 