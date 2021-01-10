# epub-boilerplate

To build an EPUB from Markdown files use following command:

```bash
pandoc -o my_book.epub --css ./pandoc.css --table-of-contents chapter1.md chapter2.md --epub-embed-font=~/.fonts/f/FiraCode_Regular.ttf --metadata title='My EPUB with code'
```

Be warned that EPUB has issues with rendering long code blocks (and EPUB viewers may differ wastly in this regard). For books with source code it's preferable to generate PDF:
```
pandoc -o my_book.pdf --css ./pandoc.css --table-of-contents chapter1.md chapter2.md --metadata title='My PDF with code'
```
