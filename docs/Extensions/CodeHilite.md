# CodeHilite

[CodeHilite](https://python-markdown.github.io/extensions/code_hilite/) is an extension that adds syntax highlighting to code blocks and is included in the standard Markdown library. The highlighting process is executed during compilation of the Markdown file.

## Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
 markdown_extensions:
 - markdown.extensions.codehilite:
      guess_lang: false 
      linenums: true # this will Add Line Numbers to Code Block
```

## Samples

### via Markdown syntax

``` VB.net
'This is Sample COde
dim a as integer
dim str as list(of String)
```
### Highlighting specific lines

``` python hl_lines="3 4"
""" Bubble sort """
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```