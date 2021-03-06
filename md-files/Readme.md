# Readme

## Table of Contents
1. [Character Syntax](#character-syntax)
1. [Text](#text)
1. [List](#list)
1. [Hyperlink](#hyperlink)
1. [Table](#table)
1. [Emoji](#emoji)

---

## Character Syntax

| Character | Syntax |
| --- | --- |
| \ | Backslash |
| ` | Backtick |
| * | Asterisk |
| _ | Underscore |
| {} | Curly Braces |
| [] | Square Brackets |
| () | Parentheses |
| # | Hash |
| + | Plus Sign |
| - | Minus Sign (Hyphen) |
| . | Dot |
| ! | Exclamation Mark |

---

## Text

1. [Insert Heading](#insert-heading)
1. [Insert Text Decoration](#insert-text-decoration)
1. [Insert Code](#insert-code)
1. [Insert Embeded Code](#insert-embeded-code)
1. [Insert Highlighted Code](#insert-highlighted-code)
1. [Insert Quotation](#insert-quotation)

### Insert Heading

You can use `# (Hash)` before the text to insert heading. The smaller number of hash, the larger heading is.

**Example**

```
# h1 tag with one hash
## h2 tag two hashes
### h3 tag three hashes
#### h4 tag four hashes
##### h5 tag five hashes
###### h6 tag six hashes
```

### Insert Text Decoration

You can cover the text with `* (Asterisk)` or `_ (Underscore)` to italicize the text.

You can cover the text with `** (Asterisks)` or `__ (Underscores)` to bold the text.

You can cover the text with `~~ (Tilde)` to insert strike-throughs.

**Example**

```
*Italicize text with asterisk*

_Italicize text with underscore_

**Bold text with asterisks**

__Bold text with asterisks__

~~Strike-Through with tlides~~
```

**Result**

*Italicize text with asterisk*

_Italicize text with underscore_

**Bold text with asterisks**

__Bold text with asterisks__

~~Strike-Through with tlides~~

### Insert Code

You can cover the text with `` ` (Backtick)`` to insert the code or command.

You can cover the text with ` ``` (Backticks)` to insert the code blocks.

**Example**

````
`Code or Command`

```
Line 1
Line 2
Line 3
``` 
````

**Result**

`Code or Command`

```
Line 1
Line 2
Line 3
``` 

### Insert Embeded Code

You can cover the code with ` `` ` to insert code inside the code.

You can cover the code block with `` ` `` or ` ```` ` to insert the code block inside the code block. If the largest number of backticks used is four, then you should use five backticks.

Backtick functions as a text if only one of them is used.

**Example**

`````
`` `Embeded Code` ``

````
```
Embeded
Code
Block
```
````

`
`````

**Result**

`` `Embeded Code` ``
````
```
Embeded
Code
Block
```
````
`

### Insert Highlighted Code

You can insert the name of language to highlight the syntax in the code.

**Example**

````
```javascript
function highlightSyntax(arg) {
  if (arg) {
  } else {
  }
}
```

```python
def highlightSyntax():
  if (arg):
    return 1
   else:
    return 0
```
````

**Result**

```javascript
function highlightSyntax(arg) {
  if (arg) {
  } else {
  }
}
```

```python
def highlightSyntax():
  if (arg):
    return 1
   else:
    return 0
```

### Insert Quotation

You can use `> (Right Angle Bracket)` before the text to insert quotation.

**Example**

`> Quoting Text`

**Result**

> Quoting Text

---

## List

1. [Ordered and Unordered List](#ordered-and-unordered-list)
1. [Task List](#task-list)

### Ordered and Unordered List

You can use `* (Asterisk)` before the text to insert unordered list.

You can use `1. 2. 3.` before the text to insert ordered list. Instead, `1. 1. 1.` works as well.

If you insert tab before the asterisk or the number, then you can indent the list.

**Example**

````
```
* Unordered
* List
  1. Indented
  2. List
1. Ordered
2. List
  * Indented
  * List
```
````

**Result**

* Unordered
* List
  1. Indented
  1. List
1. Ordered
2. List
  * Indented
  * List

### Task List

You can use `[] (Square Brackets)` before the text to insert task list. If you insert `x` between the sqare brackets, then the box will be filled with a tick. The list works if hyphen is inserted before the squared brackets.

**Example**

```
- [x] Completed Task
- [ ] Incomplete Task
```

**Result**

- [x] Completed Task
- [ ] Incomplete Task

---

## Hyperlink

1. [Insert Link](#insert-link)
1. [Insert Image](#insert-image)
3. [Insert Reference](#insert-reference)

### Insert Link

You can use `[TEXT](URL)` to insert link to the text. Replace TEXT with your own text and URL with link you want. You have three types of hyperlink:

* Heading inside markdown file
  * Replace URL with hash and a title like `#link`
  * If a title has space in between, then replace it with a dash like `#insert-link`
  * If a title has capitalized letter, then replace it with lowercase
  * The title shouldn't have any special text
* File inside repository
  * Replace URL with a directory like `/md-files/Readme.md`
* Any website
  * Replace URL with a link

**Example**

```
[Hyperlink One](#insert-link)
[Hyperlink Two](/README.md)
[Hyperlink Three](https://lee00286.github.io/portfolio)
```

**Result**

[Hyperlink One](#insert-link)

[Hyperlink Two](/README.md)

[Hyperlink Three](https://lee00286.github.io/portfolio)

### Insert Image

You can use `![TEXT](URL)` to insert image. Replace TEXT with any text and URL with link of the image.

### Insert Reference

You can use `[TEXT][1]` to apply reference. Replace TEXT with your own text.

**Example**

```
Insert [reference][1] to the [hyperlink][2]

[1]: #insert-reference
[2]: /md-files/Readme.md
```

**Result**

Insert [reference][1] to the [hyperlink][2]

[1]: #insert-reference
[2]: /md-files/Readme.md

---

## Table

You can use `- (Hyphen)` to separate the Header and cell. `| (Pipe)` is used to Separate columns. The first and last pipes can be skipped.

You can use `: (Colon)` to adjust the alignment.

* If a colon is inserted left, then column is left-aligned
* If a colon is inserted right, then column is right-aligned
* If colons are inserted both end, then column is center-aligned

:point_up: [Tables Generator](https://www.tablesgenerator.com/markdown_tables) will generate the table code for you.

**Example**

```
| Left-Aligned | Center-Aligned | Right-Aligned |
| :----------- | :------------: | ------------: |
| Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell |
```

**Result**

| Left-Aligned | Center-Aligned | Right-Aligned |
| :----------- | :------------: | ------------: |
| Content Cell | Content Cell | Content Cell |
| Content Cell | Content Cell | Content Cell |

---

## Emoji

You can use `:EMOJICODE:` to insert emoji. You can find EMOJICODES from [EMOJI CHEAT SHEET](https://www.webfx.com/tools/emoji-cheat-sheet/).

**Example**

```
| Emoji | Emojicode | Usage |
| ----- | ----- | ----- |
| :sparkles: | `:sparkles:` | Emphasize |
| :zap: | `:zap:` | Risk |
| :exclamation: | `:exclamation:` | Important |
| :question: | `:question:` | Question |
| :memo: | `:memo:` | Note |
| :point_up: | `:point_up:` | Remember |
| :warning: | `:warning:` | Warning |
| :boom: | `:boom:` | Danger |
```

**Result**

| Emoji | Emojicode | Usage |
| ----- | ----- | ----- |
| :sparkles: | `:sparkles:` | Emphasize |
| :zap: | `:zap:` | Risk |
| :exclamation: | `:exclamation:` | Important |
| :question: | `:question:` | Question |
| :memo: | `:memo:` | Note |
| :point_up: | `:point_up:` | Remember |
| :warning: | `:warning:` | Warning |
| :boom: | `:boom:` | Danger |
