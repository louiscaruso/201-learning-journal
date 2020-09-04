# Read 14


## What Google Learned about teams
- Studies also show that people working in teams tend to achieve better results and report higher job satisfaction
- Many of today’s most valuable firms have come to realize that analyzing and improving individual workers ­— a practice known as ‘‘employee performance optimization’’ isn’t enough. 
- ‘‘Teams are more effective when everyone is friends away from work. It turned out no one had really studied which of those were true.’’ -Abeer Dubey. I don't agree with this because at some point two or more friends will butt heads and the team can essentially lose its close adhesion. One of the rules of business is to never work with friends or family due to this reason. What do you think?
- Project Aristotle was organized to study hundreds of Google’s teams and figure out why some stumbled while others soared
- "Group norms" are the traditions, behavioral standards and unwritten rules that govern how we function when we gather
- Google’s data, from Project Aristotle, indicated that psychological safety, more than anything else, was critical to making a team work

## Transformation
- Transform Syntax
```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```
- 2D Rotate a box

```
HTML
<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>

```

```
CSS
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}
```

- Combining Transforms 
  - It's common for multiple transforms to be used at once 
  - To combine transforms, list the transform values within the transform property one after the other without the use of commas

```

.box-1 {
  transform: rotate(25deg) scale(.75);
}
.box-2 {
  transform: skew(10deg, 20deg) translateX(20px);
}
```
## Transitions and Animations
- One evolution with CSS3 was the ability to write behaviors for transitions and animations without the use of javascript.
- For a transition to take place, an element must have a change in state, and different styles must be identified for each state- :hover, :focus, :active, and :target pseudo-classes.
- Properties:
  - background-color
  - border-width
  - clip
  - font-weight
  - height
- Transition duration
  - `transition-duration: .2s, 1s;`
- To set multiple points at which an elements transition use
  - @keyframes Rule

```
  @keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```

## CSS Tricks
- Inset Border
```.border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}
```
- 3D Shadow
```
.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}
``` 