# Daily Read 04

## Links 
- Links are created using the `<a>` element
- The `<a>` element uses the href attribute to indicate the page you are linking to
- If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs
- You can create links to open email programs with an email address in the "to" field
- You can use id attribute to target elements within a page that can be linked to
```
<a href="http://www.metal.com">
```
## Layout
- A `<div>` element often is used to contain elements to group together sections of a page
- browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning
- The float property moves content to the left or right of the page and can be used to create muilt-column layouts
- Pages can be fixed width or liquid (stretchy) layouts
- Designers keep pages within 960- 1000 pixels wide  and indicate what the site is about within the top 600 pixels 
- Grid helps create professional and flex designs
- CSS frameworks provide rules for common task
- You can include mulitple CSS files in one page

## Functions
```
function greeting() {
  var today = new Date();
  var hourNow = today.getHours();
  var greeting;
  if (hourNow > 18) {
    greeting = 'Good Evening!';
  } else if (hourNow > 12) {
    greeting = 'Good Afternoon!';
  } else if (hourNow > 0) {
    greeting = 'Good Morning!';
  } else {
    greeting = 'Welcome traveler!';
  }
  return document.write('<h3>' + greeting + '</h3>');
}
```
## Pair Programming
- Greater efficiency
- Engaged collaboration
- Learning from fellow students
- Social skills
- Job interview readiness
- Work environment readiness


