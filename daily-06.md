# Daily Read 06

## Object Literals

## What is an Object?
- Objects group together a set of variables and functions to create a model of something
- Variables become properties 
- Functions become methods
  - ```
  var hotel = {
    name: 'Quay',
    rooms: 40,
    booked: 25,
    gym: true,
    roomTypes:['twin', 'double', 'suite'],
    checkAvaivlability: function(){
      return this.rooms - this.booked;
    }
  };
  ```
- The `checkAvailability` is a function but when part of an object it is a method

## Document Object Model (DOM)

- The browser represents the page using a DOM tree
- DOM trees have four types of nodes: document node, element nodes, attrubute nodes, and text nodes
- You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax
- Whenever a DOM querycan return more than one node, it will always return a NodeList
- From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques
- An element node can contain multiple text nodes and child elements that are siblings of each other
- In older browsers, implementation of the DOM is inconsistent 
- Browsers offer tools for viewing the DOM tree