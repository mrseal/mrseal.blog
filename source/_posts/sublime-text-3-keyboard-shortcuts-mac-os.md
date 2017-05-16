---
title: Sublime Text 3 Keyboard Shortcuts (Mac OS)
date: 2017-05-16 18:25:32
tags: [sublime, text editor, tools, shortcuts]
categories: Tools
---

https://www.sublimetext.com/

### Basics

|   Keys   |    Commands   |
|----------|:-------------:|
| cmd + shift + l | split selection into lines |
| cmd + d |  select a word<br/>select next occurance of the word |
| cmd + left click | place multiple cursors |
| cmd + left arrow | move cursor to begining of the line |
| cmd + right arrow | move cursor to end of the line |

<!-- more -->

### Line and Indentation

|   Keys   |    Commands   |
|----------|:-------------:|
| cmd + ctrl + up/down | move line vertically |
| cmd + shift + d | duplicate line |
| ctrl + shift + k | delete line |
| cmd + [ or ] | indent line |
| cmd + shift + v | paste and indent | 

|   Menu   |    Commands   |
|----------|:-------------:|
| Edit - Line - Reindent | format the indentation |


### Goto

When you have a folder opened in sublime, you will see the folder structure in the side panel

|   Keys   |    Commands   |
|----------|:-------------:|
| cmd + p | Goto anything  e.g. go to a file in the folder |

Operators in Goto Search Box

| Operators |    Commands   |  Shortcuts  |
|-----------|:-------------:|:-----------:|
| &lt;file&gt; | Goto file |  |
| @&lt;symbol&gt; | Jump to symbol e.g. class or function |  |
| #&lt;term&gt; | Jump to term |  |
| :&lt;line_number&gt; | Jump to line number | ctrl + g |
| &lt;file&gt;@&lt;symbol&gt; | Goto the file and jump to the symbol |  |
| &lt;file&gt;#&lt;term&gt; | Goto the file and jump to the term |  |
| &lt;file&gt;:&lt;line_number&gt; | Goto the file and jump to the line number |  |

Additional

|   Menu   |    Commands   |
|----------|:-------------:|
| right click - Show Unsaved Changes... | show unsaved changes |
  

### Command Palette

Command Palette is a powerful tool where you can do many many things

|   Keys   |    Commands   |
|----------|:-------------:|
| cmd + shift + p | open the command palette e.g. reverse, sort, set syntax (HTML, Markdown etc) |


**Package Manager**

1. Search "Sublime Text Package Manager" in google, and go to "Installation" page. Follow the instructions to install package manager in your sublime.
2. Open command palette (cmd + shift + p), type "Install Package", and look for the package you want to install.


### Others

|   Keys   |    Commands   |
|----------|:-------------:|
| alt + left click drag | column selection |
| ctrl + shift + w | wrap selection with tag |