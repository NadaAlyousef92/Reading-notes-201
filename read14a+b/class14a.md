# **Read this article on CSS Transforms**

1. Transforms

There are two-dimensional and three-dimensional transforms
- 2D Transforms(work on the x and y axes, known as horizontal and vertical axes).
its inclouding (2D Rotate,2D Scale,2D Translate,2D Skew,Shorthand 3D Transforms)
- 3D Transforms(Three-dimensional transforms work on both the x and y axes, as well as the z axis. These help define not only the length and width of an element, but also the depth.)

2. Transform Syntax

This including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

3. Combining Transforms

 To combine transforms, list the transform values within the transform property one after the other without the use of commas.

4. Transform Origin

 property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.

5. Perspective

The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements, while the other includes using the perspective property on the parent element residing over child elements being transformed.

6. Transform Style

 property needs to be placed on the parent element, above any nested transforms. 
[link](http://www.css3files.com/transform-rotate/)
[link](https://24ways.org/2010/intro-to-css-3d-transforms)
[link](https://webkit.org/blog-files/3d-transforms/transform-style.html)
[link](https://dev.opera.com/articles/understanding-the-css-transforms-matrix/)
[link](https://css-tricks.com/almanac/properties/b/backface-visibility/)
[link](https://developer.mozilla.org/en-US/CSS/transform-function)

## **Transitions & Animations**

1. a transition to take place, an element must have a change in state, and different styles must be identified for each state.The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target
Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.
2. One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

Transitions
As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

In the example below the box will change its background color over the course of 1 second in a linear fashion.

Transition Demo

Vendor Prefixes
The code above, as with the rest of the code samples in this lesson, are not vendor prefixed. This is intentionally un-prefixed in the interest of keeping the code snippet small and comprehensible. For the best support across all browsers, use vendor prefixes.

For reference, the prefixed version of the code above would look like the following.

Transitional Property
The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the transition-property value will be affected by any transitions.

In the example above, the background property is identified in the transition-property value. Here the background property is the only property that will change over the duration of 1 second in a linear fashion. Any other properties included when changing an element’s state, but not included within the transition-property value, will not receive the transition behaviors as set by the transition-duration or transition-timing-function properties.

If multiple properties need to be transitioned they may be comma separated within the transition-property value. Additionally, the keyword value all may be used to transition all properties of an element.

Transition Property Demo

Transitional Properties
It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint. A handful of the more popular transitional properties include the following.

Transition Duration Demo

Transition Timing
The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration from the transition-duration property a transition can have multiple speeds within a single duration. A few of the more popular keyword values for the transition-timing-function property include linear, ease-in, ease-out, and ease-in-out.

The linear keyword value identifies a transition moving in a constant speed from one state to another. The ease-in value identifies a transition that starts slowly and speeds up throughout the transition, while the ease-out value identifies a transition that starts quickly and slows down throughout the transition. The ease-in-out value identifies a transition that starts slowly, speeds up in the middle, then slows down again before ending.

Each timing function has a cubic-bezier curve behind it, which can be specifically set using the cubic-bezier(x1, y1, x2, y2) value. Additional values include step-start, step-stop, and a uniquely identified steps(number_of_steps, direction) value.

When transitioning multiple properties, you can identify multiple timing functions. These timing function values, as with other transition property values, may be declared as comma separated values.

Transition Timing Demo

Transition Delay
On top of declaring the transition property, duration, and timing function, you can also set a delay with the transition-delay property. The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. As with all other transition properties, to delay numerous transitions, each delay can be declared as comma separated values.

Transition Delay Demo

Shorthand Transitions
Declaring every transition property individually can become quite intensive, especially with vendor prefixes. Fortunately there is a shorthand property, transition, capable of supporting all of these different properties and values. Using the transition value alone, you can set every transition value in the order of transition-property, transition-duration, transition-timing-function, and lastly transition-delay. Do not use commas with these values unless you are identifying numerous transitions.

To set numerous transitions at once, set each individual group of transition values, then use a comma to separate each additional group of transition values.

Demo

Animations
Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

Animations Keyframes
To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

Vendor Prefixing the Keyframe Rule
The @keyframes rule must be vendor prefixed, just like all of the other transition and animation properties. The vendor prefixes for the @keyframes rule look like the following:

@-moz-keyframes@-o-keyframes@-webkit-keyframes
The animation above is named slide, stated directly after the opening @keyframes rule. The different keyframe breakpoints are set using percentages, starting at 0% and working to 100% with an intermediate breakpoint at 50%. The keywords from and to could be used in place of 0% and 100% if wished. Additional breakpoints, besides 50%, may also be stated. The element properties to be animated are listed inside each of the breakpoints, left and top in the example above.

It is important to note, as with transitions only individual properties may be animated. Consider how you might move an element from top to bottom for example. Trying to animate from top: 0; to bottom: 0; will not work, because animations can only apply a transition within a single property, not from one property to another. In this case, the element will need to be animated from top: 0; to top: 100%;.

Animations Keyframes Demo
Hover over the ball below to see the animation in action.

Animation Name
Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value. The animation-name declaration is applied to the element in which the animation is to be applied to.

Using the animation-name property alone isn’t enough though. You also need to declare an animation-duration property and value so that the browser knows how long an animation should take to complete.

Animation Duration, Timing Function, & Delay
Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. To start, animations need a duration declared using the animation-duration property. As with transitions, the duration may be set in seconds or milliseconds.

 timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively. The values for these properties mimic and behave just as they do with transitions

Animation Demo
Hover over the ball below to see the animation in action.

Customizing Animations
Animations also provide the ability to further customize an element’s behavior, including the ability to declare the number of times an animation runs, as well as the direction in which an animation completes.

Animation Iteration
By default, animations run their cycle once from beginning to end and then stop. To have an animation repeat itself numerous times the animation-iteration-count property may be used. Values for the animation-iteration-count property include either an integer or the infinite keyword. Using an integer will repeat the animation as many times as specified, while the infinite keyword will repeat the animation indefinitely in a never ending fashion.

Shorthand Animations
This is accomplished with one animation property, rather than multiple declarations.

### **8 simple CSS3 transitions that will wow your users**
1. Fade in: Fade in effects are coded in two steps: first, you set the initial state; next, you set the change
2. Change color: with all kinds of math involved in calculating separate RGB values and then recombining them. we just set the dives class to 'color' and specify the color we want in our CSS.
3. Grow and Shrink: To grow an element, you have to use its width and height, or its padding.we can use CSS3s transform to enlarge.
4. Rotate elements: ne of the best is transforming the rotation of an element. Give your div the class 'rotate' and add the following to your CSS.
5. Square to circle: transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the border-radius property.
6.3D shadow: This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.
7. Swing: This animation simply moves the element left and right
8. Inset border: One of the hottest button styles is the ghost button,a button with no background and a heavy border.

***There are websites using animation***
[link](https://codepen.io/retyui/pen/ByoaXV)
[link](https://codepen.io/akshaychauhan/pen/oAfae)
[link](https://codepen.io/kieranfivestars/pen/MYdQxX)
[link](https://codepen.io/dp_lewis/pen/gCfBv)
