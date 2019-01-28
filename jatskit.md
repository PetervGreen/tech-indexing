# JATS

Support for Journal Article Tag Suite is main immediate necessity so working papers get picked up by archives and indexing. Initially designed for publishers to provide "version of record" for archives. Now becoming dominant form for scientific articles. 

https://jats.nlm.nih.gov

The JATS-List is probably the place to search for answers and then to ask questions:

https://jats.nlm.nih.gov

But first see its FAQ link which in turn links to:

http://www.mulberrytech.com/JATS/

Will do separate bibliography. Meanwhile wiki page below has useful links. 

## JATSKit

This looks like a plausible starting point. Works with oXygen. Author/editor needs to have licensed copy (USD $100 for academic institution).

oXygen editor includes this framework:

https://www.oxygenxml.com/doc/versions/20.1/ug-editor/topics/author-jats-doc-type.html

So installation instruction below only needed for installing latest development version instead of current stable version.

Article explaining what this is about:

https://www.ncbi.nlm.nih.gov/books/NBK350379/

Note: above article is published in an ebook style. Clicking the cogwheel icon for settings generates a printable version that can be printed locally to pdf. Both are generated from same static web site using the JATS standard and software promoted by the US National Center for Biomedical Information which published the article. Aim is to use JATSKit and related software to produce similar documents online.


Article links to descriiption of customized implementation for a journal publisher.

Also links to video demo of installing a framework in oXygen which is well worth watching:

https://www.oxygenxml.com/demo/FrameworkConfiguration.html

Above starts with explanation of what any framework adds to simply using an XML editor.

Later includes full details for adding customizations to oXygen. It is worth knowing about the possiibility of doing customizations for later but actual installation of either the stable or latest version of JATSKit is much simpler using the
installation link below and unnecessary since JATSKit is now included with oXygen.

See all wiki pages for documentation:

https://github.com/wendellpiez/JATSKit/wiki

Especially:

installation:

https://github.com/wendellpiez/JATSKit/wiki/Installation

and note limitations:

https://github.com/wendellpiez/JATSKit/wiki/Limitations

Will need to find solution for pdf output limitation if not already fixed. But learning how to install and use this looks like good starting point for anything else.

## Markdown

Will need separate support for use of markdown both for drafting and collaboration revising initial drafts quickly and to include references from shared Zotero bibliography.

Assumption: this will use pandoc with zotxt to generate an XML file that can then be enhanced and published using oXygen and JATSKit as above. It should be relatively easy to sort that out once we have actual experience with JATSKit above.

Use of pandoc-jats (with Zotero) would be next priority after familiarizing with installed JATSKit.

Other journals may require different citation styles from those for NCBI submissions included with JATSKit. Pandoc can use any journal's CSL file as supported by  Zotero. 

Note: There may complications as pandoc-jats uses a special "XML" citation style,

## DITA

Support for writing small markdown topics separately and using dita maps etc to combine them into articles is highly desirable for reasons to be explained elsewhere.

Assumption: it will be easier to figure out how to do this using DITA-OT to output a single normalized LwDITA markdown document and then convert to JATS XML using pandoc.

Meanwhile can still start writing small topic files and combine them manually into draft papers for input to pandoc.

Not found anything on LwDITA in search of JATS-List.

## Tools

Jatswiki.org is down. Last update to list of tools was 2017-10-30 archived six months later:

http://web.archive.org/web/20180426004313/http://jatswiki.org/wiki/Tools

Still useful but out of date so need to find a list that is continuously updated.



