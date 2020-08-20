# Daily Read 09

## Forms

### Why?
- Google's search box is a form

### Structure
- Form controls live inside a `<form>` element
- Should have the `<action>` attribute
  - It's value is a URL for the page on the server that will receive the info
- Will usually have method and id attribute as well
  - Forms can be sent using: get or post
    - Post: appends form-data inside the body of the HTTP request (data is not shown in URL),
Has no size limitations, Form submissions with POST cannot be bookmarked
    - Get: Appends form-data into the URL in name/value pairs,
The length of a URL is limited (about 3000 characters),
Never use GET to send sensitive data! (will be visible in the URL),
Useful for form submissions where a user wants to bookmark the result,
GET is better for non-secure data, like query strings in Google
- Input element is used to create several different form contols, the value of the type attribute determines what kind of input they will be creating
```
<input type="text" name="username" size="15" maxlength="30" />
```
- Input types:
```
<input type="button">
<input type="checkbox">
<input type="number">
<input type="password">
<input type="radio">
<input type="submit">
<input type="text">
```
- Label can be used in two ways
  - Wrap around both the text description and form input 
  - Be kept separate from control and use the `for=""` attribute to indicate which form control and it is label for
- Fieldset the can group related form controls together, helps with longer forms 
- Legend element can come directly after the opening `<fieldset>` 

## Lists, Tables and Forms
- There are several properties that control specifically forms, tables, and forms
- List markers can be given different appearances using the list-style-type and list-style image properties
- Table cells can have different borders and spacing in different browers, but there are properties you can use to comtrol them and make them more comsistent
- Forms are easier to use if the form controls are vertically aligned using CSS
- Forms benefit form styles that make them feel more interactive

## Events

### What are events
- When your browse the web, your browser registers different types of events. It's the browser's way of saying "Hey, this just happened." Then your script can respond.
- Different types of events:
  - UI event
  - Keyboard event
  - Mouse event
  - Focus event
  - Forms event
  - Mutation event

### How they trigger JavaScript Code
- Select the element node(s) you want the script to respond to 
- Indicate which event on the selected node will trigger the response
- State the code you want to run when the event occurs

### Event Listeners
```
fuction checkUsername() {
  // code to check the username  
}
var el = document.getElementById('username');
el.addEventListener('blur', checkUsername, false);
```
