---
title: Sublime Text 3 Keyboard Shortcuts (Mac OS + Windows)
date: 2017-05-16 18:25:32
tags: [sublime, text editor, tools, shortcuts]
categories: Tools
---

https://www.sublimetext.com/

### Basics

|   Mac OS   |   Windows   |   Commands   |
|------------|:-----------:|:------------:|
| cmd + shift + l | ctrl + shift + l | split selection into lines |
| cmd + d | ctrl + d | select a word<br/>select next occurance of the word |
| cmd + left click | ctrl + left click | place multiple cursors |
| cmd + left arrow | home | move cursor to begining of the line |
| cmd + right arrow | end | move cursor to end of the line |

<!-- more -->

### Line and Indentation

|   Mac OS   |   Windows   |   Commands   |
|------------|:-----------:|:------------:|
| cmd + ctrl + up/down | ctrl + shift + up/down | move line vertically |
| cmd + shift + d | ctrl + shift + d | duplicate line |
| ctrl + shift + k | ctrl + shift + k | delete line |
| cmd + [ or ] | ctrl + [ or ] | indent line |
| cmd + shift + v | ctrl + shift + v | paste and indent | 

|   Menu   |    Commands   |
|----------|:-------------:|
| Edit - Line - Reindent | format the indentation |


### Goto

When you have a folder opened in sublime, you will see the folder structure in the side panel

|   Mac OS   |   Windows   |   Commands   |
|------------|:-----------:|:------------:|
| cmd + p | ctrl + p | Goto anything  e.g. go to a file in the folder |

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

|   Mac OS   |   Windows   |   Commands   |
|------------|:-----------:|:------------:|
| cmd + shift + p | ctrl + shift + p | open the command palette e.g. reverse, sort, set syntax (HTML, Markdown etc) |


**Package Manager**

1. Search "Sublime Text Package Manager" in google, and go to "Installation" page. Follow the instructions to install package manager in your sublime.
2. Open command palette (cmd + shift + p), type "Install Package", and look for the package you want to install.  There's a few interesting packages such as Color Highlighter, Emmet (nice autofill tool for html, css ...) etc.

|   Mac OS   |   Windows   |   Commands   |
|------------|:-----------:|:------------:|
| ctrl + w | shift + ctrl + g | wrap with Emmet |

### Others

|   Mac OS   |   Windows   |   Commands   |
|------------|:-----------:|:------------:|
| alt + left click drag | shift + right click drag | column selection |
| ctrl + shift + w | alt + shift + w | wrap selection with tag |