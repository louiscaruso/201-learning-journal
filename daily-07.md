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
```
The script is placed inside an immediately invoked function expression
   which helps protect the scope of variables 

(function() {

  // PART ONE: CREATE HOTEL OBJECT AND WRITE OUT THE OFFER DETAILS

  // Create a hotel object using object literal syntax
  var hotel = {
    name: 'Park',
    roomRate: 240, // Amount in dollars
    discount: 15,  // Percentage discount
    offerPrice: function() {
      var offerRate = this.roomRate * ((100 - this.discount) / 100);
      return offerRate;
    }
  };

  // Write out the hotel name, standard rate, and the special rate
  var hotelName, roomRate, specialRate;                    // Declare variables

  hotelName = document.getElementById('hotelName');        // Get elements
  roomRate = document.getElementById('roomRate');
  specialRate = document.getElementById('specialRate');

  hotelName.textContent = hotel.name;                      // Write hotel name
  roomRate.textContent =  '$' + hotel.roomRate.toFixed(2); // Write room rate
  specialRate.textContent = '$' + hotel.offerPrice();      // Write offer price

// PART TWO: CALCULATE AND WRITE OUT THE EXPIRY DETAILS FOR THE OFFER
  var expiryMsg; // Message displayed to users
  var today;     // Today's date
  var elEnds;    // The element that shows the message about the offer ending

  function offerExpires(today) {
    // Declare variables within the function for local scope
    var weekFromToday, day, date, month, year, dayNames, monthNames;

    // Add 7 days time (added in milliseconds)
    weekFromToday = new Date(today.getTime() + 7 * 24 * 60 * 60 * 1000);

    // Create arrays to hold the names of days / months
    dayNames = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
    monthNames = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'];

    // Collect the parts of the date to show on the page
    day = dayNames[weekFromToday.getDay()];
    date = weekFromToday.getDate();
    month = monthNames[weekFromToday.getMonth()];
    year = weekFromToday.getFullYear();

    // Create the message
    expiryMsg = 'Offer expires next ';
    expiryMsg += day + ' <br />(' + date + ' ' + month + ' ' + year + ')';
    return expiryMsg;
  }

  today = new Date();                             // Put today's date in variable
  elEnds = document.getElementById('offerEnds');  // Get the offerEnds element
  elEnds.innerHTML = offerExpires(today);         // Add the expiry message

// Finish the immediately invoked function expression
}());
```