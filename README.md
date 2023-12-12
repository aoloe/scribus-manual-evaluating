# Evaluating Scribus

Currently, we have a "work in progress" first draft version as the <en/README.md>.

If you want to contribute, please read <CONTRIBUTE.md>.

## Creating the documents

### Epub

Creating the Epub with pandoc:

```
pandoc README.md --metadata-file=pandoc-epub/metadata.yaml --css=pandoc-epub/epub.css -o out/evaluating-scribus.epub
```

Notes:

- reference for the epub css: https://github.com/jgm/pandoc/blob/main/data/epub.css



## TODO

- [ ] Should we look for a better title for the document?
- [ ] Create a make file that produces the output files
- [ ] Create a script that converts the data between Github and Cryptpad
