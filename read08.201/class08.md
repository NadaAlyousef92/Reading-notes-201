# **Layout**

**Key concepts in positioning elements**

1. **Building blocks**

CSS treats each HTML element as if it is in its own box.This box will eaither be a block-level box or an inline box
+block-level elements:start on a new line ex(< h1 > < p > < ul > < li >)
+inline elements: flow in between surrounding text ex(< img > < b > < i >)

2.**Containing elements**:
if one block level element sits inside another block-level element then the outer box is known as the containing or parent element

3.**controllong the position elements**:
Css has the folowing positioning schemes that allow you to control the layout of a page for example:
+Normal flow
+Relative positioning(allow shifting elements all sides and didnot affect the position of sirrounding elements)
+fixed positioning(a form of absolute positioning that positions the element in relasion to the browser window as opposed to the containing element, elements dont affect the position of surrounding elements and they dont move while scrolling up and down)
+absolute positioning(let moveing as a users scrolling up and down the page)
+floating elements(allow you to take that element out of normal flow and position it to the far left or right of a containing box)

- < div > element are often used as containing elements to group togather sections of a page.
Browsers display pages in normal flow unless you specify relative,absolute or fixed positioning.
-The float property moves content to the left or right on the page and can be used to create multi-column layouts.(floating items require a defined width).
-Pages can be fixed width or liquid (strechy)layouts.
-Designers keep pages within 960-1000 px wide and indicate what the site is about within the top 600px (to demonstarte its relevence without scrolling).
-Grides help create professional and flexible designs.
-CSS Framworks provide rules for common tasks.
-you can include multiple CSS files in one page.
