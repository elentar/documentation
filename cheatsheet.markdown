---
layout: default
title: Markdown Cheatsheet
published: true
sorting: 1
alias: markdown-cheatsheet.html
---

Markdown formatting is simple, and the CFEngine generator adds a few things
to make it even simpler. Here's a list of the most commonly used formats.

## Basic Formatting

`**Bold**` **Bold**

`*Italic*` *Italic*

## Links

### Link within documentation and to known pages

`[top of the page][Markdown Cheatsheet] and [inside page][Markdown Cheatsheet#Link within documentation]`

[top of the page][Markdown Cheatsheet] and [inside page][Markdown Cheatsheet#Links]

**Note:** For known pages, see the 
[_references.markdown](https://github.com/cfengine/documentation-generator/blob/master/_references.md)
file.

### Link to CFEngine keyword

The documentation pre-processor will create those automatically.

```
`classes` and `readfile()`
```

`classes` and `readfile()`

### Link to External URL

`[Markdown Documentation](http://daringfireball.net/projects/markdown/)`

[Markdown Documentation](http://daringfireball.net/projects/markdown/syntax)


## Lists

Unordered lists - Markdown supports other markers than the asterisk, but in 
CFEngine we use only `*`.

```
* Item 1
* Item 2
   * Item 2a
* Multi paragraph item

    Four spaces indented
```

* Item 1
* Item 2
   * Item 2a
* Multi paragraph item

    Four spaces indented



Ordered lists - the numbers you use don't matter.

```
1. first
1. second
9. Third
```

1. first
1. second
9. Third

## Code

### Code Blocks

You need to keep an empty line in front of the code block!

    ```
        $ code block
        $ without syntax highlighting
    ```

```
    $ code block
    $ without syntax highlighting
```

    ```cf3
        # CFEngine block
    
        bundle agent example()
        {
        }
    ```

```cf3
    # CFEngine code block

    bundle agent example()
    {
    }
```

### Inline code

    This renders as `inline code`.

This renders as `inline code`.

*****

## Headers

`# Level 1`

# Level 1

`## Level 2`

## Level 2

`### Level 3`

### Level 3

`#### Level 4`

#### Level 4

`##### Level 5`

##### Level 5

`###### Level 6`

###### Level 6

*****