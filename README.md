# Markdown Cheatsheet for VS Code


## Index
- [Headings](#headings)
- [Paragraph](#paragraph)
- [Emphasis](#emphasis)
- [Lists](#lists)
- [Links](#links)
- [Images](#images)
- [Code](#code)
- [Other Elements](#other-elements)
- [Blockquotes](#blockquotes)
- [Tables](#tables)


&nbsp;
## **Background**


This cheatsheet can be used when writing Markdown in Visual Studio Code.

To use markdown in VS Code:
1. Install the `markdownlint` extension.
2. Create a new file and save with the `.md` extension.
3. Open the Markdown Preview window:
    + On Mac --> Press <kbd>&#8984;</kbd>+<kbd>K</kbd> then <kbd>V</kbd>
    + On Windows --> <kbd>Ctrl</kbd>+<kbd>K</kbd> then <kbd>V</kbd>
4. Start writing Markdown 😊


&nbsp;
## **Headings**

The following markdown represents the standard HTML `<h1>` to `<h6>` elements.  Short notation is to use `#`, but you can also hardcode the heading tags: 


```
# H1
## H2
### H3
#### H4
##### H5
###### H6

<h6> H6 In HTML tags </h6>
```

# H1 with auto underline...
## H2
### H3
#### H4
##### H5
###### H6

<h6> H6 In HTML tags </h6>


&nbsp;
## **Paragraph**

### A plain paragraph
```
Just a plain paragraph, nothing special here.
```
Just a plain paragraph, nothing special here.  

&nbsp;
### An empty line

```
An empty line:
&nbsp;
```
An empty line:
&nbsp;

&nbsp;
### A horizontal line
```
---
```

---



&nbsp;
## **Emphasis**

```
**Bold**

_Italic_

**_Bold and Italic_**

~~Strikethrough~~
```

**Bold**

_Italic_

**_Bold and Italic_**

~~Strikethrough~~

&nbsp;
## **Lists**

### Ordered List (use numbers)

```
1. First item
2. Second item
3. Third item
    1. This must start form "1" again.
    2. Indented item
    99. The value doesn't matter here. Renders as "3".
4. Fourth item
```

1. First item
2. Second item
3. Third item
    1. This must start form "1" again.
    2. Indented item
    99. The value doesn't matter here. Renders as "3".
4. Fourth item

### Unordered List (can use - + or *)

```
- First item
- Second item
- Third item
    + Indented item
    + Indented item
* Fourth item
* Fifth item
```

- First item
- Second item
- Third item
    + Indented item
    + Indented item
* Fourth item
* Fifth item


&nbsp;
## **Links**

### Named hyperlink
```
[Google](https://www.google.com)
```

[Google](https://www.google.com)

&nbsp;
### Automatically converted links
```
This link will also work - https://www.google.com.
```

This link will also work - https://www.google.com.

&nbsp;
### Anchor links
```
[Index](#index)
```
[Index](#index)


&nbsp;
## **Images**

### Inline-style

```
![alt text](https://github.com/IllusiveMilkman/markdown_cheatsheet_for_vs_code/blob/main/img/lost.png?raw=true "Inline")
```

![alt text](https://github.com/IllusiveMilkman/markdown_cheatsheet_for_vs_code/blob/main/img/lost.png?raw=true "Inline")


&nbsp;
### Referenced like a variable

```
![alt text][logo]

[logo]: https://github.com/IllusiveMilkman/markdown_cheatsheet_for_vs_code/blob/main/img/lost.png?raw=true "Referenced"
```

![alt text][logo]

[logo]: https://github.com/IllusiveMilkman/markdown_cheatsheet_for_vs_code/blob/main/img/lost.png?raw=true "Referenced"


&nbsp;
### An image link

```
[![alt text](https://github.com/IllusiveMilkman/markdown_cheatsheet_for_vs_code/blob/main/img/lost.png?raw=true "Image link")](https://unsplash.com/)
```

[![alt text](https://github.com/IllusiveMilkman/markdown_cheatsheet_for_vs_code/blob/main/img/lost.png?raw=true "Image link")](https://unsplash.com/)


&nbsp;
## **Code**

### Inline code

```
Remember to use the appropriate `<h1>` heading.
```

Remember to use the appropriate `<h1>` heading.

&nbsp;
### Code blocks
Basic code block without syntax highlighting by using three backtics ```` ``` ```` before and after your codeblock.

````
```
<div>
  <p>Test</p>
</div>
```
````

```
<div>
  <p>Test</p>
</div>
```

&nbsp;
### Syntax Highlighting


Merely add your language after the backticks to enable syntax highlighting, e.g.

### html

````
```html
<div>
  <p>Test</p>
</div>
```
````

```html
<div>
  <p>Test</p>
</div>
```

&nbsp;
### javascript

````
```javascript
const numbers = [1,2,3];
numbers.forEach( number => {
    console.log(number);
});
```
````

```javascript
const numbers = [1,2,3];
numbers.forEach( number => {
    console.log(number);
});
```

&nbsp;
### Ruby

````
```ruby
def fuel(🥛)
  return 🍪
end
```
````

```ruby
def fuel(🥛)
  return 🍪
end
```


&nbsp;
## **Other Elements**

### Abbreviations
```
<abbr title="Laugh Out Loud">LOL</abbr> is short for... (hover your mouse over the abbreviation).
```

<abbr title="Laugh Out Loud">LOL</abbr> is short for... (hover your mouse over the abbreviation).

&nbsp;
### Subscript
```
H<sub>2</sub>O
```
H<sub>2</sub>O

&nbsp;
### Supercript
```
X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>
```
X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

&nbsp;
### Keyboard keys
```
Press <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd> to end the session.
```
Press <kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd> to end the session.

&nbsp;
### Highlights
```
One can <mark>highlight text</mark> in markdown. 
```

One can <mark>highlight text</mark> in markdown. 



&nbsp;
## **Blockquotes**

#### Blockquote without attribution

```
> It is a miracle that curiosity survives formal education.
```

> It is a miracle that curiosity survives formal education.

&nbsp;
#### Blockquote with attribution

```
> It is a miracle that curiosity survives formal education.
>
> — <cite>Albert Einstein</cite>
```

> It is a miracle that curiosity survives formal education.
>
> — <cite>Albert Einstein</cite>


&nbsp;
## **Tables**

Tables are designated by `|` (pipe character).  There are a few things to note:
* alignment for the column is designated by `:` (colon).
* If no colon is specified, it will default to left alignment.
* Spaces within cells are ignored as well.
* Outer pipes are optional.
* One can use inline markdown within cells


```
| Column 1      | Column 2      | Column 3  |
| :------------ |:-------------:| ---------:|
| left          | center        | right     |
| left | center| right |
1 | 2 | 3
_Italic_ | `inline code` | **Bold**
```


| Column 1      | Column 2      | Column 3  |
| :------------ |:-------------:| ---------:|
| left          | center        | right     |
| left | center| right |
1 | 2 | 3
_Italic_ | **Bold** | `<div>`
