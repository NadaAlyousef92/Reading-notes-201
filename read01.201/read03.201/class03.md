# Lists in HTML
-**ordered lists:**are lists where each item in the list is numbered its created with the < ol >element.-

-**unordered lists:**are lists that begin with a bullet point (rather than characters that indicate orders).its created with the<ul>element.

-**definition lists:**are made up of the set of terms a long with the definition for each of those terms.
its ceated with the < dl >element and usually consist of a series of terms and their definitions.
< dt >this is used to contain the term being defined (the definition term)
< dd >this is used to contain the definition -

-**Nestes lists:**its created with < li >tag stands for lists items and for create a sub-list or nesred list

## Boxes
-CSS treats each HTML elements as if it has its own box.
-you can use CSS to control the dimensions of a box.
-you can control also the borders,margin ans padding for each box with CSS.
-it is possible to hide elements using the display and visility properties.
-block-level boxes can be made into inline boxes and inline boxes made into block-level boxes.
-legibility can be improved by controlling the width of boxes containing text and the leading.
-CSS3 has introduced the ability to create image,borders ans rounded borders.


### **switch statements**
-starts with a variable called the switch value. each casr indicates a possible value for this and the code that should run if the variable matches that value.

**IF...ELSE**
*there is no need to provide an else option (you can just use an if statement)*
*with a series of **if** statements they are all checked even if a match has been found (so its perform slowly than switch)*

**switch**

-the porpose of using switch statenment is to present the user with a different message depending on which level they are at.The message is stored in a variable called msg.


*There are a default option that is run if noone of the cases match.*
*If a match is found that code is run ;then the break statement stop the rest of the switch statement running (provide better performance than multiple if statements)*

**switch statement syntax**

switch (level1) {

case 'one':
title = 'level 1';
break;

case 'two':
title = 'level 2';
break;

case 'three':
title = 'level3';
break;

default:
title = 'test';
break;

}

#### **Truthy and falsy value**

-falsy values are treated as if they are false.The table to the left shows a highscore variable with a series of values, all of which are falsy.and it can be treated as anumber 0.

-Truthy values are treated as if they are true. ALmost everything that is not in the falsy table can treated as if it were true.And it can be treated as a number 1 .

**There are three types of loops (for , while ,and do) each repeats a set of statement.***
