# PyMarkdown Extension

PyMdown Extensions is a collection of extensions for Python Markdown. Keep in mind, the PyMdown extensions were designed to work with the default extensions, so your mileage may vary in regards to compatibility when paired with other 3rd party extensions.

## Critic

 [Critic](https://facelessuser.github.io/pymdown-extensions/extensions/critic/) implements [Critic Markup](http://criticmarkup.com/), a Markdown extension that enables the tracking of changes (additions, deletions and comments) on documents. During compilation of the Markdown document, changes can be rendered (default), accepted or rejected.

### Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
markdown_extensions:
 - pymdownx.critic
```

### Samples
- {==Highlight Text==}
- {++Addition++} New Text
- {--Deletion --} Old Text
- {>>Comment <<}
- {~~hipsum~>ipsum~~}

{==

Formatting can also be applied to blocks, by putting the opening and closing
tags on separate lines and adding new lines between the tags and the content.

==}

## Caret 

Caret optionally adds two different features which are syntactically built around the `^` character. The first is **insert** which inserts ``. The second is **superscript** which inserts `` tags.

### Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
markdown_extensions:
 - pymdownx.caret
```

### Sample Code

- ^^Text with underLine^^

- H^2^0

- text^a\ superscript^

## InlineHilite

[InlineHilite](https://facelessuser.github.io/pymdown-extensions/extensions/inlinehilite/) adds support for inline code highlighting. It's useful for short snippets included within body copy

### Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
markdown_extensions:
 - pymdownx.inlinehilite
```

### Sample Code

- `#!js var test = 0;`
- `#!VB.net dim a as integer`

## Mark

Mark adds the ability to insert `` tags. The syntax requires the text to be surrounded by double equal signs. 

### Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
markdown_extensions:
 - pymdownx.mark
```

### Sample Code

- ==This is Highlighted==

## MagicLink

MagicLink is an extension that provides a number of useful link related features. MagicLink can auto-link HTML, FTP, and email links. It can auto-convert repository links (GitHub, GitLab, and Bitbucket) and display them in a more concise, shorthand format. MagicLink can also be configured to directly auto-link the aforementioned shorthand format.

### Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
markdown_extensions:
 - pymdownx.magiclink
```

### Sample Code

- Just paste links directly in the document like this: https://google.com.
- Or even an email address: fake.email@email.com.

## Task List

The Tasklist extension adds GFM style task lists. They follow the same syntax as GFM. Simply start each list item with a square bracket pair containing either a space (an unchecked item) or a x (a checked item).

### Installation

Add the following lines to your `mkdocs.yml`:

``` yaml
markdown_extensions:
 - pymdownx.tasklist
```
### Sample Code
Task List

* [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
* [x] Nulla lobortis egestas semper
* [x] Curabitur elit nibh, euismod et ullamcorper at, iaculis feugiat est
* [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [x] Sed egestas felis quis elit dapibus, ac aliquet turpis mattis
    * [ ] Praesent sed risus massa
* [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque
* [ ] Nulla vel eros venenatis, imperdiet enim id, faucibus nisi

## Emoji

Emoji adds the ability to insert a :shit: ​load of emojis that we use in our daily lives.

```yaml
markdown_extensions:
  - pymdownx.emoji:
      emoji_index: !!python/name:pymdownx.emoji.twemoji
      emoji_generator: !!python/name:pymdownx.emoji.to_svg
```

