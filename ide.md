# Integrated Development Environment

Initial thoughts on working environment while catching up on more than two decades of rapid technical progress.

Help wanted. Anbody passing by, please let me know of other links I should be looking at. (Fork or use issue tracker).

Indexing and a lot of other work should be based on XML pipelines using an XML database.

Authors input documents in (extensions of) markdown, word processor documents, Zotero bibliographies, forms or scraped from web sites etc.

Pipelines of simple python scripts ingest into Xml database eg with:

https://palletsprojects.com/p/click/ and/or:

https://palletsprojects.com/p/flask/

Some examples of simple python scripts, not using XML database pipeline, have been forked into [translation-embeddings](https://github.com/thecapitalistcycle/translation-embeddings)

Rest of processing done with IDEs and XML pipelines for DITA to publish in multiple versions and channels.

This architecture is strikingly similar to other basic principles for robusness, maintainability, scalability and resilience eg: 

1. FLAMEGPU use of pipelined communicating state machines where operations run in parallel on high performance GPU cluster.
Data accessed by each operation as independent from others as possible. Likely to be using that with ABM models of economy.

2. RESTful web APIs. Used everwhere.

3. Publish and Subscribe Message Oriented Middleware. Especially with MMORPGs.

Several IDEs seem to be directly or indirectly relevant to most of our authoring and development work.

1. Eclipse - generally essential. Especially for interactive UML animation.
2. oXygen - heavy duty XML editing. Likely to be useful with DITA
3. IntelliJ IDEA. Supports current Andoid SDK and pycharm which could be useful for python work eg with Flask.
https://en.m.wikipedia.org/wiki/IntelliJ_IDEA

All three integrate with BaseX XML database. From Wikipedia article that looks plausible as first choice.

Only interested in local interactive use initially. Different database technology required for high performance online (eg CouchDB).

## Xproc

https://www.w3.org/TR/xproc/

BaseX may not directly support Xproc so also consider eXist (but its implementation of Xproc looks old).

There are various implementations of Xproc:
http://xproc.org/implementations/

with tests:

https://github.com/xproc/1.0-test-suite

review test results:
https://github.com/xproc/1.0-test-suite/tree/xproc10/results

There are ways to use BaseX with Xproc eg at CXAN:
http://cxan.org/about
http://cxan.org/pkg/fgeorges/calabash-basex
http://xmlcalabash.com/docs/
http://cxan.org/pkg/fgeorges/pipx
http://pipx.org

There are also various proposed and accepted extensions for both XProc and XSLT:
http://exproc.org
http://exslt.org




