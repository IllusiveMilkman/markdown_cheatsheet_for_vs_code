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

This cheatsheet can be used as a reference for writing Markdown in Visual Studio Code.

Recently, I started taking coding notes in VS Code, using Markdown.  It allows me to focus on the content and code without becomming bogged down with style or syntax highlighting.  I'm sure there are other mechanisms, but this one works for me.

Since the result of your notes is a file or set of files, you can then save however you prefer, like in cloud storage or even a private Github repository.

### Setup

To use markdown in VS Code:

1. Install the `markdownlint` extension.
2. Create a new file and save with the `.md` extension.
3. Open the Markdown Preview window:
    - On Mac --> Press <kbd>&#8984;</kbd>+<kbd>K</kbd> then <kbd>V</kbd>
    - On Windows --> <kbd>Ctrl</kbd>+<kbd>K</kbd> then <kbd>V</kbd>
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
### Relative links
```
[The relative.md file](relative.md)
```
[The relative.md file](relative.md)



&nbsp;
## **Images**

Below are examples of images generated from full URL paths or relative paths:

&nbsp;
### Displaying an image

```
![random image](https://source.unsplash.com/random/100x100)
```

![random image](https://source.unsplash.com/random/100x100)

But what if your source image is too large and you only want to set a specific size? In those cases you can write HTML directly to specify image sizes.  You can set height and width. Setting only a **single** height or width and keep the _aspect ratio_ of the original image:

Original image at 300 x 300:

```
![random image](https://source.unsplash.com/random/300x300)
```

![random image](https://source.unsplash.com/random/300x300)

Same image at but now source is scaled to 200 x 200:

```html
<img src="https://source.unsplash.com/random/300x300" width="200" height="200" alt="Resized image in HTML"/>
```

<img src="https://source.unsplash.com/random/300x300" width="200" height="200" alt="Resized image in HTML"/>

&nbsp;
### An image link

```
[![alt text](https://source.unsplash.com/random/100x100 "Image link")](https://unsplash.com/)
```

[![alt text](https://source.unsplash.com/random/100x100 "Image link")](https://unsplash.com/)


&nbsp;
### Referenced (like a variable)

```
![alt text][logo]

[logo]: img/lost.png "Referenced"
```

![alt text][logo]

[logo]: img/lost.png "Referenced"



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
_Italic_ | **Bold** | `<div>`
```


| Column 1      | Column 2      | Column 3  |
| :------------ |:-------------:| ---------:|
| left          | center        | right     |
| left | center| right |
1 | 2 | 3
_Italic_ | **Bold** | `<div>`
