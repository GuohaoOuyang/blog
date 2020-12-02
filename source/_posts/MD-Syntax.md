---
title: MD Syntax
comments: true
date: 2020-11-29 21:09:52
updated: 2020-11-29 21:09:52
categories: Syntax
tags: [Markdown, Note]
---
#### Headings
```
# Heading level 1 => <h1>Heading level 1</h1>
## Heading level 2 => <h2>Heading level 2</h2>
...til ######(6)
```

#### Bold
```
**bold text** => <strong>bold text</strong>
```

#### Italic
```
*cat's meow* => <em>cat's meow</em>.
```
<!--More-->
#### Bold and Italic
```
***really important*** => <strong><em>really important</em></strong>
```

#### Horizontal Rules

``*** || --- ``

---

#### Strikethrough


```
~~The world is flat~~
```
~~The world is flat~~

#### Escape
`\* Without...`
\* Without the backslash, this would be a bullet in an unordered list.

#### Blockquotes
```
> Dorothy followed her through many 
>
> ... with  Multiple lines
>> with nested blockquotes 
```
> Dorothy followed her through many 

#### Ordered Lists
```
1. First item
7. Second item
3. Third item
    1. Indented item
    2. Indented item
outer number not important
```
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item

#### Unordered Lists
```
* || + || - First item
* || + || - Second item
* || + || - Third item
keep consistent
```

#### Code Block
with indent (1 or 2 tabs)

    <html>
        <head>
        <title>Test</title>
    </head>

without indent (escape)
````
```
<html>
    <head>
    <title>Test</title>
</head>
```
````

#### Table
```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

#### Task List
```
- [x] Write the press release
- [ ] Update the website
```
- [x] Write the press release
- [ ] Update the website

#### Definition List
```
First Term
: This is the definition of the first term.
```
First Term
: This is the definition of the first term.


#### Links & Emails
with title
`
[title](url)
`
[title](#url)

without title
`<fake@example.com>`
<fake@example.com>

#### Images
`
![title](../uploads/qie.jpg "optional title")
`
![](../uploads/qie.jpg)



