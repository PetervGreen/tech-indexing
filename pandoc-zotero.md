# Pandoc and Zotero

Most of our work will be preparing bibliographies using Zotero with plugins and previewing working papers drafted in pandoc markdowm with plugins.

Start here:

https://github.com/pandoc-scholar/pandoc-scholar

https://www.zotero.org/support/plugins

https://www.zotero.org/support/

https://pandoc.org/press.html

https://github.com/jgm/pandoc

These notes are mainly about the interaction between the two. I do not have any current experience and it will be necessary 
to acquire some up to date experience in order to get things right.

Drafts would be kept in a repository here and could be edited through the browser here or preferably with an editor like
Atom after pulling to writer's local platform.

There are many plugins for Atom, including the following specifically for markdown:

https://github.com/topics/atom-package?q=markdown&unscoped_q=markdown

and for git:

https://github.com/topics/atom-package?q=git&unscoped_q=git

The words "I assume" below imply "I don't know". Hopefully trying things out will clarify. Otherwise any remaining assumptions will be replaced with more detailed numbered questions for posting to places where somebody might now.

While reading docs on pandoc, zotero and other items mentioned below, please note the relevant issue trackers or other such
places where we can hope for answers and add the links here.

I assume that we and others using our bibliographies will eventually be submitting articles to journals or moderated archives which require submissions in either LaTeX or JATS as well as pdf and require the use of various different citation styles. Some publishers may want Word docx.

I assume our bibliographies will include all possible information about each citation in a neutral encoding that can be used with any CSL and submission format. Only citation keys are embedded within an article and the corresponding bibliographic details are stored in a separate json or yaml file with the same name so that the same markdown file can be used to generate whatever output is desired.

## Zotero

Bibliographies and drafting should be kept completely separate. If a new citation is found while drafting it should be added
to a specific Zotero bibliography and assigned a short key to use in the draft. If a doi, ISBN etc is available I assume this can be used within Zotero to automatically add all fields. If necessary an incomplete stub should be put in Zotero to be 
completed later. We always eventually find and include all such fields as doi, isbn and md5 (from Library Genesis) to be able
to retrieve and update full details later.

Individual bibliographies should be regularly merged with a master including all to resolve any key conflicts.

If offline the minimum necessary details for Zotero should be put in a note within the draft to fix later.

I assume that markdown footnotes would be used for all citations.

Some journals may (as Modelewski, 1967 noted at p35-6) prefer stupid inline citations like the example in this sentence.

Adaptations for that should be considered later when we actually have to deal with it. Meanwhile footnotes are simpler.

I assume zotxt would be used to pull citations from Zotero into the markdown file.

https://github.com/egh/zotxt

This has features for including page numbers and other text together with the citation that I do not understand and
may also be relevant to inline citations.

I do not understand the reference to "Zotxt API". I assume this is access proided by Zotero as a server on the local host to zotxt as a client so that the client can pull citation data from Zotero using the keys it reads.

I assume Better BibTeX for Zotero would be used as recommended by zotxt.

I assume this avoids any problems arising from the differences between LaTeX and other usage of Zotero citations.

https://github.com/retorquere/zotero-better-bibtex

I assume pandoc-citeproc would be used together with CSL stylesheets specific to each journal.

https://github.com/jgm/pandoc-citeproc/blob/master/man/pandoc-citeproc.1.m

https://github.com/jgm/pandoc-citeproc

Note that there are currently 37 open issues, some recent, some 2014 as well as 291 closed issues at:

https://github.com/jgm/pandoc-citeproc/issues

## Pandoc

I assume that any tricks learned while trying out pandoc with Zotero can and should be automated for future use
by turning them into snippets of a YAML file as described here:

https://heerdebeer.org/Software/markdown/pandocomatic/

I assume that careful study of the above manual, together with the full pandoc manual and the docs for other items mentioned above is necessary to be able to handle regular publishing to multiple journals.

I am not planning to do that study but can help by studying particular bits referred to me while solving particular problems.

Give exact paragraph references to docs not understood in an issue describing the problem that points to a folder with the exact files for recreating the problem and the exact command line that triggers it.

## JATS

At Github currently there are 17 repositories on topic "jats":

https://github.com/topics/jats

456 on topic "pandoc"

My guess is that the ridiculous numbers for pandoc are from individuals solving specific problems they have preparing articles for particular journals. Many of these problems may involve JATS.

Somewhere in there, nearly every problem we are likely to encounter will have been dealt with.

Carefully reading the relevant documents listed above for Pandoc and Zotero in advance is likely to save a LOT of trouble and make it easier to locate and understand any other items needed.

We should only tackle JATS issues after having got a basic ability to preview pdf of a pandoc markdown article in any citation style.

I assume that when we do it will involve using pandoc for markdown input to jats output. Then using a jats verifyer.

Perhaps also viewing and editing the jats output with an XML editor (preferably oXygen).

Then using pandoc for jats input to pdf output for preview.

This looks relevant for verifying:

https://github.com/PeerJ/jats-conversion

This will be even more relevant and their recommendations should be studied carefully before starting drafts for JATS.

https://jats4r.org

Relevance greater because "reuse" relates directly to DITA.

## DITA

I do not understand how to combine JATS and DITA.

My guess is that we would use:

http://www.dita4publishers.org

together with

https://github.com/dita-for-small-teams

plus custom XSL to output JATS.

No point thinking about it until we are confident with Zotero, Pandoc and JATS.

However I will be pointlessly "thinking about it" while writing actual content in small markdown topics for sections and
glossary entries etc in the hope that these could eventually be turned into MDITA for LwDITA instead of just cut and pasted.

No guarantee this will ever be productive (whereas Zotero, pandoc and JATS will certainly be useful).

The effort required to install d4st is considerable but mainly involves sysadmin skills that will be generally useful.

I have forked it here so we could add notes for others while learning such skills and asking for help to get it working.

https://github.com/thecapitalistcycle/dita-for-small-teams

If considering it, start with the docker tutorial to actually deploy a working app that uses redis for backend data:

https://docs.docker.com/get-started/

https://redis.io

This is ONE component:

https://github.com/sameersbn/docker-redis/blob/master/README.md

of the dockerized GitLab:

https://github.com/sameersbn/docker-gitlab

that is a major part of d4st.

Another, bigger, component of GitLab is:

https://github.com/sameersbn/docker-postgresql

Understanding the installation for d4st is less daunting if you are aware it is avoiding having to do the full installation for the above but only the specific tweaks they mention.

Trying out the above components first may be helpful (or may not).

But I would take this slowly, reading up on all the new concepts rather than blindly following. We won't be able to use it for quite a while and any experience with Zotero/pandoc/JATS will be higher priority.





