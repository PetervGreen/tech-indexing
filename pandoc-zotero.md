# Pandoc and Zotero

## Zotero

Most of our work will be preparing bibliographies using Zotero and previewing working papers drafted in pandoc markdowm.

These notes are mainly about the interaction between the two. I do not have any current experience and it will be necessary 
to get some up to date experience in order to get things right.

Drafts would be kept in a repository here and could be edited through the browser here or preferably with an editor like
Atom after pulling to writer's local platform.

Bibliographies and drafting should be kept completely separate. If a new citation is found while drafting it should be added
to a specific Zotero bibliography and assigned a short key to use in the draft. If a doi, ISBN etc is available I assume this can
be used within Zotero to automatically add all fields. If necessary an incomplete stub should be put in Zotero to be 
completed later. We always eventually find and include all such fields as doi, isbn and md5 (from Library Genesis) to be able
to retrieve and update full details later.

Individual bibliographies should be regularly merged with a master including all to resolve any key conflicts.

If offline the minimum necessary details for Zotero should be put in a note within the draft to fix later.

I assume that markdown footnotes would be used for all citations.

Some journals may (as Modelewski, 1967 noted at p35-6) prefer stupid inline citations like the example in this sentence.

Adaptations for that should be considered later when we actually have to deal with it. Meanwhile footnotes are simpler.

I assume zotxt would be used to pull citations from Zotero into the markdown file

I assume pandoc-cite would be used together with CSL stylesheets specific to each journal.
