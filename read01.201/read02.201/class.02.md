# Text in HTML

***Structural markup:*** the elements that you can use to describe both heading anf paragraphes


1.**Headings**

*HTML has six levels of heading depends on its priority ans importance to the text
from h1 to h6*

2.**Paragraphes**

*Aparagraph consist of one or more sentences that form a self-contained unit of discourse, the start of paragraph is indicated by anew line.*

***To create a paragraph surround the words that make it with an opening< p > tag and closing < /p > tag.***

3.***BOld and Italic***

-By enclousing words in the tags< b >and< /b> we can make characters apear bold.

-By enclousing words in the tags < i > and < /i> we can make characters appear in italic.

4.**Superscript and Subscript**

-The <  sup > element is used to contain characters that should be superscript such as the suffixes of dates or mathmatical concepts

-The < sub > element is used to contain characters that should be subscript it is commonly used with foot notes or chemical formulas

5.**Line breaks and Horizontal rules**

-<  p >----< /br >---< /p > :the browser will automatically show each new paragraph or heading on anew line.(the line break tag </br>.

-< p >---< /p >< hr/ >----< p >---< /p > :to create a break between themes such as achange of topic in a book or anew scene in aplay you can add horizontal rule between sections using the <hr/>tag.

6.**Visual editors and their code views**

-Visual editors often resemble word processors although each editor will differ slightly,there are some features common to most editor allow you to control the presentation of text.

-Code views show you the code created by the visual editor so you can manually edit it.


***Semantic markup***: its an elements that arenot intended to affect the structure of web pages but they do add extra inf to the pages; such as where emphasis is placed in a sntence,that something you have written is a quotation(and who said),the meaning of acroyms-- etc.


7. **strong and emphasis**
-The use of the < strong > element indicates that its content has a strong importance 
-The < em > element indicates emphasis that subtly changes the meaning of a sentence

8. **Qoutations**
-THe < blockquote > element is used for longer quotes that take up an entire paragraph
-The < q > element is used for shorter quotes that sit within a paragraph.

9. **Abbreviations and acronyms**
-The < abbr > element can be used A tittle attribute on the openning tag is used to specify the full term 
-In HTML4 there was a separate < acronym > element for acronyms to spell out the full form of the acronym.

10.**Citations and Definitions**
-The < cite > element used to indicate where the citation is from when you are referencing a piece of work such as a book.
-The < dfn > element is used to indicate the defining instance of a new term.

11.**Author details**

*The < address > element has quite a specefic use to contain contact details for the author of the page.

12.**Changes to content**
-The < ins > element used to show content that has been inserted into a document while the <del> element can show text that has been deleted from it.
-The < s > element indicates something that is no longer accurate or relevant (but that shouldnot be deleted), its usually displayed whith a line through the center.


## Color

1.How to specify colors
2.color terminology and contrast
3.background color

-Color not onlu bring your site to life , but also helps convey the mood and evokes reactions.

-There are three ways to specify colors in CSS:
1.RGB values:
2.hex codes:
3.color names:

-Color pickers can help you to find the color you want

-there is enough contrast between any text and background color(otherwise people wont be able to read your content.

-CSS3 has introduced an extra value for RGB colors to indicate opacity .its known as RGBA.

-CSS3 allows you to specify colors as HSL values with an optional opacity value its known as HSLA.


### Decisions and loops

*Switch statements allow you to compare a value against possible outcomes(and also provides a default option if none match*
-Using switch statements: the purpose of the switch statement is to present the user with different message depending on which level they are at the message is stored in a veriable called msg.

-The veriable called level 1 contains a number indicating which level the user is on .this is then used as the switch value (the switch value could also be an expression).

-In the following code block (inside the curely braces),there are three options for what the value of the level variable might be the number 1,2or3.

*each level ends with the break keyword which will tell the javascript inrtptrter to skip the rest of this code block and continue onto the next.
