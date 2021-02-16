# Forms

-Whenever you want to collect information from visitors you will need a form, which lives inside a < form > element.
-Information from a form is senr in name/value pairs.
-Each form control is given a name and the text the user types in or the value of the options they select are sent to the server.
-HTML5 introduces new form elements which make it easier for visitors to fill in forms.

## lists ,tables and forms

-There are severals CSS properities used to control the appearance of lists,tables and forms
-Lists makers can be given different appearances using the list-style-type and list-style image properties
-Table cells can have different borders and spacing in different browsers but there are properties you can use to control them and make them more consistent 
-Forms are easier to use if the form controls are vertically algned using CSS
-forms benefit from styles that make them feel more interactive

### lists

-**ordered lists:**are lists where each item in the list is numbered its created with the < ol>element.

-**unordered lists:**are lists that begin with a bullet point (rather than characters that indicate orders).its created with the<ul>element.

-**definition lists:**are made up of the set of terms a long with the definition for each of those terms.
its ceated with the < dl>element and usually consist of a series of terms and their definitions.
< dt>this is used to contain the term being defined (the definition term)
< dd>this is used to contain the definition

-**Nestes lists:**its created with < li>tag stands for lists items and for create a sub-list or nesred list

#### Tables

* A table represents information in gride format for example (TV,schedules and sports result)*

-The < table > element is used to add tables to web page

-A table is drown out row by row ,Each row is created with the < tr > element

-Inside each row there are anumber of cells represented by the < td > element (or < th > if it is a header)

-you can make cell of a tabel span more than one row or column using the rowsoan and colspan  attributes

-for long tables you can split the table into a < thead >,< thbody >, and < tfoot >

##### Events

-Events are the browser way to indicating when something has happened (such as when a page has finished loading or a button has been clicked)
-Binding is the process of stating which event you are waiting to happen and which element you are waiting for that event to happen upon.
-When an event occurs on an element it can trigger a javaScript function ;When this function then changes the web page in some way .it feels interactive beause it has responded to the user.
-You can use event delegation to monitor for events that happen on all of the children of an element
The most commonly used of events are W3CDOM events,Although there are others in the HTML5 specification as well as browser-specific events 