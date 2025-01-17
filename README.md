# Flix Highlight.js Language Spec

This is the official repository for the Flix language specification
for [highlight.js](https://highlightjs.org/).

## Table of contents
- [Build](#Build)
- [Use](#Use)

## Build

### Using GitHub workflow

If you fork this repository there is a GitHub workflow
that on each push will automatically build a minimal
highlight.js file that only supports Flix for the web.

Additionally, it also generates a Flix spec that can be appended
to an existing highlight.js file.

The GitHub workflow always targets the latest release of
highlight.js

### Manual installation

We refer you to
[the official documentation for 3rd party grammars for highlight.js](https://GitHub.com/highlightjs/highlight.js/blob/main/extra/3RD_PARTY_QUICK_START.md#testing)
(read Testing & Packaging sections).

## Use

The highlight.js file built by the GitHub workflow
should work automatically when included on a website.

### Custom styling

We use mdBook for [doc.flix.dev](https://doc.flix.dev/) which
has some custom styling rules (see [css files](https://github.com/flix/book/tree/master/theme))
This is to properly highlight string interpolation among
other things.

| Selector      | Description                                |
|---------------|--------------------------------------------|
| `.hljs-subst` | Used for highlighting string interpolation |
| `.hljs-meta`  | Used for highlighting annotations          |

