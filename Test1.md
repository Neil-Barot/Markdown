# This is Markdown

## Paragraphs
Writing paragraphs in markdown is as simple as simply typing.

Additional paragraphs can be added by performing a double enter. One enter simply acts as a space.

You can add a \<br> by adding two spaces after a line and pressing enter.   
Ex: test


## Headings
Use the hash(#) symbol to create headings. Each hash corresponds to a header  
Ex: \#\# = \<h2>

## Text Effects
There are various text effects available in Markdown. Examples and the code required are shown below.  

**bold**: **test** - surround text with \*\*bold** double astericks or press control B after

**Italics**: *test* - surround text with \*italics* single astericks or press control I after the word.

**Crossed off**: ~~test~~ - surround text with \~~crossed~~ double tilde's

**Highlight**: <mark>test</mark> - use the HTML tag \<mark>Highlighted\</mark>

**Superscript**: X<sup>2</sup> - use the HTML tag \<sup>Superscript\</sup>

**Subscript**: H<sub>2</sub>O - use the HTML tag \<sub>Subscript\</sub>

## Code Blocks
```js
    const a = 10
    // comment
    let y = 8
``` 

To have a code block, surround the block of code with \``` Code \```. Keep the ticks on different lines surrounding the code block. 

You can add the language after the first ticks to get language apprpriate highlighting.  
Ex: \```js for Javascript or \```py for python


## Creating Links
[This is a link](/Test1.md): To make a link, add text inside of a square bracket and the destination for the link inside of parentheses.  
Ex: \[This is a link]\(/Test1.md) This just created a link to the Test1.md file in my local directory.

## Adding Images
Adding images follows a similar protocol, except you add an exclamation point before.  
Ex: \!\[ Alt Text ]\( Image link ) 

![alt text](Example1.jpg)