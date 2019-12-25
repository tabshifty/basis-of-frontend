### Markdown

A quick shot for markdown. To learn in detail, click this [link](https://daringfireball.net/projects/markdown/)

#### Paragraph and break
one or more blank lines to separate paragraphs  
one or more spaces to break lines

#### Headers
Numbers of # respresent 1-6 header levesl, like this:

	# This is an H1  
	## This is an H2  
	### This is an H3

#### Blockquotes
Markdown use > for blockquoting  
Blockquotes can contain other markdown elements

#### Lists
_*_ _+_ _-_ all the same used for unordered lists  
Nunbers are used for ordered list

#### Code blocks
To produce a code block in Markdown, simply indent every line of the block by at least 4 spaces or 1 tab. Dont forget to insert blank line before code blocks.  
A code block continues until it reaches a line that is not indented (or the end of the article).

#### Horizontal rules
Three or more _*_ _-_ _\__ will produce a Horizontal rule tag

#### Links
To create an inline link, use a set of regular parentheses immediately after the link text’s closing square bracket. Inside the parentheses, put the URL where you want the link to point, along with an optional title for the link, surrounded in quotes. For example:

	This is [an example](http://example.com/ "Title") inline link.
	[This link](http://example.net/) has no title attribute.
If you’re referring to a local resource on the same server, you can use relative paths:

	See my [About](/about/) page for details.  
Reference-style links use a second set of square brackets, inside which you place a label of your choosing to identify the link:

	This is [an example][id] reference-style link.
#### EMPHASIS
Text wrapped with one _\*_ or _\__ will be wrapped with an HTML `<em>` tag  
Double _\*_’s or _\__’s will be wrapped with an HTML `<strong>` tag.

#### Code
To indicate a span of code, wrap it with backtick quotes _\`_

#### Images
Inline image syntax looks like this:

	![Alt text](/path/to/img.jpg)
	![Alt text](/path/to/img.jpg "Optional title")
#### Blackslash escapes
Markdown allows you to use backslash escapes to generate literal characters which would otherwise have special meaning in Markdown’s formatting syntax  
Markdown provides backslash escapes for the following characters:

	\   backslash
	`   backtick
	*   asterisk
	_   underscore
	{}  curly braces
	[]  square brackets
	()  parentheses
	#   hash mark
	+   plus sign
	-   minus sign (hyphen)
	.   dot
	!   exclamation mark
[Back2md](#markdown)
______________________

### Github
Go straightly to this [link](https://git-scm.com/book/en/v2) for detailed content

#### Basic Command
`git init`  Initialize an existing directory  
`git clone`  Clone an existing repository, rename like this`git clone http://* newname`  
`git status`  Check status of files
`git add`   Track untracked files or stage modified files, this command can add all files in a directiory recursively  
`git commit`  commit staged changes, this will launch an editor. Use flag `-m` to commit message inline.The `-a` flag automatically stage every tracked files to skip `git add` part    
``