# Contribute to this tutorial

You can contribute by:

- Proof reading the English version or a translation.
- Creating and adding content (according to the "Questions we want to answer" below).
- Translating into other languages.

... Or other things we didn't even think about.

## Basic informations for contributors

### How to edit "Evaluating Scribus"

- This document _home_ is on Github:
  - <https://github.com/aoloe/scribus-manual-evaluating>
  - For those who are not comfortable with Github, we also provide a collaborative pad  that is kept in sync with Github (as long as somebody is editing it):  
    https://cryptpad.fr/code/#/3/code/view/f01f7d85c02a35c6eb55661f331ffd0c/
- If you want to edit this document with Git (Github):
  - Fork <https://github.com/aoloe/scribus-manual-evaluating>,
  - make your changes,
  - trigger a merge request.
- If you want to edit this document on [CryptPad](https://cryptpad.fr):
  - Create an account on CryptPad.
  - Ask in the Scribus community to become a contributor and post there your CryptPad username.

### The goals

- The goal of this document is
  - to convey a rough understanding about Scribus,
  - to be as short as possible,
  - not to be exhaustive.

Below, we have a list of questions this document aims at answering:

- Before adding new content (or modifying the existing content), please make sure that your contribution fits one of the questions.
- If you want do add a new question or modify an existing one, please discuss it first with the other authors (as an example in the Scribus forums or with a ticket in the Github repository).


### English skills and translations

The original of this document is the English version.

Changes to the content should first get into the English version. Since not everybody who contributes has perfect English skills:

- If you want to make changes to the content while translating (or while reading a translated version), please also add it to the English.
- If you're not feeling proficient enough, try to write very simple sentences, that are mostly correct. Somebody else can improve upon them later.
- If that is also not possible, please add a _todo note_ ("TODO: this is new content") next to your changes (if necessary, with an explanation of the reasons for the change).
  - On Github we publish releases of this document with diffs to help the translators to spot the changes in the English version.

And since nobody is perfect: You're welcome to improve other people text.

### Assets

- If you make screenshots, please provide the .sla document you're using, so that other people can easily update and translate them.
- If you create artworks (svg, xcf, odt, ...) that you use in the screenshot, please also share them.

### ... finally...

- This document is published under a CC-BY-SA license.
- Please behave in a way that is pleasant for the other contributors.

## Questions we want to answer

All the content in this document, should be answering one of the questions in this section.

If you want to add new content and it does not really fit (yet), please discuss the new topic (and question) with the other contributors.

### Is Scribus the right tool for me?

- How Scribus can match someone needs.

### What is DTP?

Just a short sentence: currently, it's a link to Wikipedia.

### How do I install Scribus?

- We might want to publish multiple versions of this document, one for each _supported_ platform.

### How / where can I can I click around in Scribus to evaluate it?

- We don't want to teach how to use Scribus
- We only want to show how the user can perform some simple tasks
- Creating text and image frames
- Basic text formatting (bold/italic/size, pick and add fonts, create and apply styles, advanced typographic settings)
- Creating pages, adding page numbers
- Linking frames
- Producing a PDF
- What is missing?

### What I can do if I'm stuck?

- Where is my font?
  - Just explain the basics, do not write a full tutorial
  - If tutorials exist, link to them

## Markdown style guide

For this document we use Markdown and we use a [syntax that is compatible with Pandoc](https://pandoc.org/MANUAL#pandocs-markdown).

### Formatting

We try to avoid special formatting and CSS classes, but if you want to use one, add a `div` or a `span` around the text that you want to style:

```md 
:::{.page-break}
A red paragraph
:::

This is black and [This is red]{.red}.
```

and add to the `epub.css` file:

```css
div.red p {
  color: red;
}
span.red {
  color: red;
}
```

Currently, the following CSS classes exist:

- `div.page-break hr`: hides the horizontal line and insert a page break before.

  ```md
  :::{.page-break}
  ---
  :::
  ```

### Images

Currently, we try to be compatible with both Pandoc and CryptPad.

Images must always be first defined in the usual Markdown style.  
For CryptPad we also need a `<media>` _internal_ link to the CryptPad driver file.

```html
![This is what Scribus looks like](what-is-scribus.png)
<!-- <media-tag src="https://files.cryptpad.fr/blob/dd/dddf90c51e3f77c23e2f95a6d942b526b462a84dc44f05dc" data-crypto-key="cryptpad:o1LB5WBGnCKDn2rnn2eh+S+TW03XRDQukQzvWQxlbvQ="></media-tag> -->
```

One of both is always enclosed in a Html comment (`<!-- -->`)

## User _complaints_

We want to build this document on real user's needs.

Here is a list of complaints people made about Scribus. Let's try to learn from them!

If you find other complaints that can help improving this document (not to improve Scribus!) please add them to this section!

As a basic guidance: we don't want to collect all user's issues, just those issues that make them wonder, why they even got into using Scribus.

### The original complaint

On December, 7 2023, [abrogard wrote to the Scribus forums](https://forums.scribus.net/index.php/topic,4778.msg22014.html):

> First off [Scribus] just looked like MS draw or something.
> then I tried pasting in some text. didn't work.
> then i opened a text box and tried again. didn't work
> then i 'inserted' and a whole file came in.
> so then i tried to embolden a heading. 
> didn't work.
> then i googled and found that won't work. got to select a different font.
> now's a good time, I think, for me to get a 'heads up'
> what do I want this for?
> which software is it an immediate improvement on?  which thing has it 'done better than they do'?
> or if you like: which costly software does it do the same as but free?
> or which need does it address that currently isn't met?
> 
> not arguing with it, you understand? not trying to put it down at all.  just simply trying to get it straight what i'm into here.  so's i don't ask what it perhaps can't deliver and perhaps was never meant to deliver.
> 
> Must admit I do very little 'desktop publishing'  mainly I do it when I have to send formatted submissions to my online school.  I find Word and Libre Office often quite bloody annoying there. Improvement on that would be good.
