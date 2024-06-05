# mdtoc-nextcloud : markdown table of contents for Nextcloud

This program generates a markdown table of contents which is clickable in Nextcloud markdown editor.

## Requirements

Most of the requirements are standard unix tools.

- `sed`
- `awk`
- `iconv`
- `grep`
- `tr`
- `paste`

## Usage

```
usage: mdtoc [-i = insert in file] <file.md>
```

The default behaviour is to output the result to stdout.

If you use the `-i` option, the table of contents will be inserted between the following markers in the source file:

```
# Some markdown file

<!--toc-->
Table of contents will be inserted here
<!--/toc-->

## Some section

Some  text
```
