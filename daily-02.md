# Daily read 02

## Chapter 02 HTML text
- HTML elements are used to describe the structure of the page
  * HTML has six levels of headings:
  ```
  <h1> This is a main heading
  <h2>
  <h3>
  <h4>
  <h5>
  <h6> This is level 6
  ```
  * More elements
    - Paragraphs `<p>` `</p>`
    - Bold `<b>` `</b>`
    - Italic `<i>` `</i>`
    - Break line `<br />`
    - Horizontal line `<hr />`
    
- Semantic Markup 
  * Strong `<strong>` indicates important text
  * Emphasis `<em>` the text to make suble changes to the sentence
  * Block quotes `<blockquote>` `</blockquote>`
  * To just quote is `<q>` `</q>`
  
## Chapter 10 Intro to CSS
- The `<link>` element can be used in HTML to tell the browser where to find the CSS file
  * `href` specifies the path to the CSS file
  * `type` attribute specifies the type of document bein linked
  * `rel` specifies the relatinship between the HTML page and the file it is linked to 
- The `<style>` you can also inclued CSS rules within an HTML page by placing it inline with a element

## CSS selectors
- Universal Selector applies to all elements in the document
  * `* ()`
- Type selector matches element names
  * `h1 h2 h3 ()`
- Class selector matched and element whose class attribute has a value that matches the one specified after the period
  * `.note ()`
- ID selectors matches an element whose id attribute has a value that matches the one specified after the pound symbol
  * `#introduction ()`   

## Basic JS 
- A script is a series of instrutions that a computer can follow step by step, known a statments
  * ```
  var today = new Date();
  var hourNow = today.getHours();
  var greeting;
  
  if (hourNow > 18) {
    greeting = 'Good evening';
  }
  else if (hourNow > 12) {
    greeting = 'Good afternoon';
  }
  else if (hourNow > 0){
    greeting = 'Good morning';
  }
  else {
    greeting = 'Welcome';
  }
  document.write(greeting);```

  * Comments `/* comment here */` for multi line comments
  * Or `// comment here //` for single line comments 
- Is the test score greater than 50
```
if (score > 50){
  document.write('You passed!');
}
else {
  document.write('Try again');
}
```

## The seven rules of git commit
- Separate subject from body with a blank line
- Limit the subject line to 50 characters
- Capitalize the subject line
- Do not end the subject line with a period
- Use the imperative mood in the subject line
- Wrap the body at 72 characters
- Use the body to explain what and why vs. how
