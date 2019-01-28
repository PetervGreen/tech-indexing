# JATS

Support for Journal Article Publishing suite is main immediate necessity so working papers get picked up by archives and indexing. Initially designed for publishers to provide version of record to archives. Now becoming dominant form for scientific articles. Will do separate bibliography.

## JATSKit

This looks like a plausible starting point. Works with oXygen. Author/editor needs to have licensed copy (USD $100 for academic institution).

Article explaining what this is about:

https://www.ncbi.nlm.nih.gov/books/NBK350379/

Video demo of installing a framework in oXygen:

https://www.oxygenxml.com/demo/FrameworkConfiguration.html

Above starts with explanation of what any framework adds to simply using an XML editor.

Later includes full details for adding customizations to oXygen. It is worth knowing about the possiibility of doing customizations for later but actual installation of either the stable or latest version is much simpler using the
installation link below.

See all wiki pages for documentation:

https://github.com/wendellpiez/JATSKit/wiki

Especially:

installation:

https://github.com/wendellpiez/JATSKit/wiki/Installation

and note limitations:

https://github.com/wendellpiez/JATSKit/wiki/Limitations

Will need to find solution for pdf output. But learning how to install and use this looks like good starting point for anything else.

## Markdown

Will need separate support for use of markdown both to draft and collaborate on initial text quickly and to include references from shared Zotero bibliography.

Assumption: this will use pandoc with zotxt to generate an XML file that can then be enhanced and published using oXygen and JATSKit as above. It should be relatively easy to sort that out once we have actual experience with JATSKit above.

Use of pandoc-jats (with Zotero) would be next priority after familiarizing with installed JATSKit.

## DITA

Support for writing small markdown topics separately and using dita maps etc to combine them into articles is highly desirable for reasons to be explained elsewhere.

Assumption: it will be easier to figure out how to do this using DITA-OT to output a single normalized LwDITA markdown document and then convert to JATS XML using pandoc.

Meanwhile can still start writin small topic files and combine them manually into draft papers for input to pandoc.
