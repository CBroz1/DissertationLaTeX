# Dissertation LaTeX

**All of the LaTeX source code to compile my dissertation.**

I used my dissertation writing process as an opportunity to learn about using LaTeX to generate pdfs. The final product should be viewed via [eScholarship.org](https://escholarship.org/uc/item/2kk8z7sx). The main document is _Broz_Dissertation.tex, and it calls upon the other tex, bib, and png files in the directory to compile the completed file.

## Quick start guide

- Download a LaTeX compiler, like TeXShop
- Test compile some example documents, including mine 
- Many compilers need to be run multiple times, including a run for BibTex
- Many files are generated in the compiling process in addition to the pdf, including .aux, .bbl, .blg, .log, etc.

## Major lessons I learned

- Make your life easier by referencing other files instead of having one big document
	- `\graphicspath` will store your images in a subfolder
	- `\input` will reference other .tex files
	- `\def` will let you alias commands
- `threeparttable` is a type that is much easier to conform to APA standards
- Tables: Does your statistics software allow you to export as plain text? Then it's theoretically possible to write a script or make an excel table that takes text and outputs tables. Whether or not this is efficient depends on how many 'final' versions of your analysis you have.
- Citation management:
	- Google scholar will give you the BibTeX of anything, if you select it in your settings
	- [JabRef](https://www.jabref.org/) can help manage notes in .bib format, and export to MS Word xls format
	- Your .bib file doesn't need to be in any order, but it *really* helps to have consistent names - and no conflicting names
	- [This](https://packagecontrol.io/packages/Indent%20Respectful%20Sort) Sublime Text package will allow you to do indent respectful sort to put your bibs in order.
- Tools for referencing other parts of your document: 
	-`\label`, `\phantomsection`, `\ref` and `\pageref`
