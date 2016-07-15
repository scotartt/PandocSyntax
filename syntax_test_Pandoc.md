<!-- SYNTAX TEST "Packages/PandocSyntax/PandocSyntax.sublime-syntax" -->

---
title: YAML Block
---

# Heading 1 {#header_id}

## Heading 2 {-}

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

### Heading 3

This paragraph has text in **bold**, *italics*, a `code block`, and an
equation: $x = y$. It also has text with sub~script~ and super^script^.
Pandoc-figref {#f:figlabel} and pandoc-chem-struct s:{CH2Cl2} are also
supported.

#### Heading 4 {-}

- This is a list with *italics*
- Item **2** of list

-   Still a list, but with multiple paragraphs in an item.

    Second paragraph.

    Third paragraph.

1. *Numbered list*
2. Numbered list

<!-- This text is part of a comment. -->

This paragraph contains a [link](\url). This is a [reference link][ref]. This
is an <inline link.html>. This is a [shortcut reference link].

![Figure](/path)

This inline ![Figure 2] has the path specified separately. Lorem ipsum dolor
sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut
labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis
aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in
culpa qui officia deserunt mollit anim id est laborum.^[inline with @citation from [p.1]]

[ref]: \url

[shortcut reference link]: \url

[Figure 2]: /path

 > A quote with *italics*. After the italics.
    That *continues* on the **next** line.
 > 
 >Next part of *quote*.

Lorem ipsum dolor sit amet,[^noteref] consectetur adipisicing elit, sed do
eiusmod tempor incididunt ut labore et dolore magna aliqua.^[Inline footnote]
Ut enim ad minim veniam,[@citation] quis nostrud exercitation ullamco laboris
nisi ut aliquip ex ea commodo consequat.[^noteref] Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.[^noteref]
Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
deserunt mollit anim id est laborum. @citation with no brackets. @citation [p.2] [-@citation p.3].

 [^noteref]: This is a *footnote*. Inline cite with page ref: -@citation [p.2] this seems to only work when indented one space.


| A line block.
|   Which will preserve *leading* spaces.

```
A fenced code block.
```

~~~
A tilde fenced code block
~~~

Or just indent code:

    Like this.

