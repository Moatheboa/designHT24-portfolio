---
Title: About
Description: The techniques of this homepage.
---

Home page
==========================

The overall structure, as in the general display of the header, navigation and footer, is written in Twig.
The content of these -text, images, icons- are found in files written in Markdown.
The styling of the page is brought by Sass.
The reason for using multiple files and languages is to separate the various functions of the code.

Markdown is a simple markup language that is used to create the content, both text and media. This can then be converted into HTML but is still easy to read before the conversion.

Twig is a template language, and generates HTML from the Markdown files. It is used for the logic part, as it allows for loops, conditions and variables to create a template that can be reused for multiple webpages. 

Sass is used to style the page and in this case it is saved in scss-files. Sass has two syntaxes. The scss-version is very similar to css. The sass-version, saved in sass-files, is a bit simpler, but might still be more complicated if you have to go in between css and sass. Sass has a little bit more functions than just plain css.
