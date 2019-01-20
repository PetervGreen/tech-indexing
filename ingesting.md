# Ingesting

DITA solves the problem of Content Management and publishing to various formats. Does not include ingestion.

## PubMed

PubMed archives have an internal workflow for accepting research papers in many formats and putting them in standard archive formats that can be read online or offline with PubMed reader software.

Not seen but presumably open source and the best place to look for solutions.

## Pdf

Difficult even for text based. Scan based presumably requires OCR first and then complex customized text processing.

That will be needed to extract indexes from old books.

Also for processing old scanned articles and perhaps some more recent ones that are only available scanned.

Apache Tika can help at least with metadata and text based. Also for many other sorts of ingestion.

https://tika.apache.org

Chris A Mattmann_ Jukka L Zitting-Tika in action-Manning Publications  (2012).pdf

@book{book:906965,
   title =     {Tika in action},
   author =    {Chris A Mattmann; Jukka L Zitting},
   publisher = {Manning Publications },
   isbn =      {9781935182856,1935182854},
   year =      {2012},
   series =    {},
   edition =   {},
   volume =    {},
   url =       {http://gen.lib.rus.ec/book/index.php?md5=987f45a2fba941e33c48c9ee02afd8a6 }
}

But they recommend Tabula for tables:

https://tabula.technology
https://github.com/tabulapdf/tabula

This is only for text based.

Tika uses PDFBox which also has many other features:

https://pdfbox.apache.org

## Word

oXygen recommends several methods including Word2DITA:

http://blog.oxygenxml.com/2016/05/how-to-migrate-from-word-to-dita.html

http://www.dita4publishers.org/d4p-users-guide/user_docs/d4p-users-guide/word2dita/word2dita-intro.html

From here, which looks **massively useful** for many other aspects. Move elsewhere to checkout thoroughly:

http://www.dita4publishers.org

https://github.com/dita4publishers

https://github.com/dita4publishers?page=2

http://www.dita4publishers.org/d4p-users-guide/

NB Also supports custom javascript in epubs and mentions that as of 2016 iBooks and Adobe Digital Editions have good support.

http://www.dita4publishers.org/d4p-users-guide/user_docs/d4p-users-guide/epub-plugin/using_custom_javascript.html

XMLmind uses w2x:

http://www.xmlmind.com/w2x/_distrib/doc/w2x_app_help/index.html

## TEI

Presumably TEI has to ingest and markup scanned originals. Have not checked out but here is one starting point:

https://github.com/TEIC

## Cinnamon

(Move this after checking out)

Open source full Enterprise Content Management System.

Don't know if has ingestion facilities but need to checkout anyway (and also look for any others)

http://www.cinnamon-cms.com

https://github.com/dewarim/cinnamon

https://sourceforge.net/p/cinnamon/code/HEAD/tree/Client/trunk/


via ditawriter.com which also needs to be checked out thoroughly:

http://www.ditawriter.com/dita-books/

See also:

https://www.g2crowd.com/categories/component-content-management-systems
