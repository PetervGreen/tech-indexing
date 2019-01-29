# DITA For Small Teams

This project appears to be exactly what I have been looking for.

No updates since 2017-04-07 pre-release 0.97 but still looks like best starting point.

https://github.com/dita-for-small-teams/dita-for-small-teams/releases

None of the previous 6 forks of main repository are updated more recently:

https://github.com/dita-for-small-teams/dita-for-small-teams/network/members

Suggests (and provides a docker configuration ready to go) for exactly
the same software stack I had in mind:

- GitLab with CI/CD (or any git with CI/CD)
- BaseX with XQuery 3 XML database
- oXygen XML Editor
- DT-OT

Writing this without looking at code. 
Not sure whether it uses Eclipse plugin for oXygen but specifically mentions XQuery 3.1.

https://github.com/dita-for-small-teams

http://www.d4st.org

Overview here:

http://www.d4st.org/topics/dita-for-small-teams.html

Supports my basic assumption:

"These are all features that are offered by commercial content management systems to one degree or another. Commercial 
CMS systems can offer a lot of value but they also represent a significant monetary and time investment, an investment that 
many teams either simply cannot make or do not have budget for early in the process of adopting DITA.

Most, if not all, of these facilities—distributed access, version management, production automation, tool integration, and 
even link management—can be provided by free or low-cost tools and services at the cost of some time spent setting up and 
maintaining the system. This makes it possible for even the smallest writing team to get the benefit of sophisticated, 
DITA-aware content management, with a very small initial investment of time and money. Most of the money spent will be on 
authoring tool licenses and most of the time spent is just getting the necessary tools and services in place: none of them 
are difficult to acquire, install, or configure."


Also claims:

"In most cases it should be possible, following the guidelines provided here, to set up a working collaborative DITA 
authoring and production environment in just a few hours.

The D4ST project’s Docker-based solution makes it about as easy as it can be to provision and use the D4ST approach. 
Docker makes it possible to package disparate tools together in a convenience but flexible way and manage them as a 
logical unit. Because each tool or supporting component is managed as a separate Docker container it is relatively 
easy to adapt the set of tools and configuration details to suit your specific needs. The same Docker containers 
can be run on a single personal machine, on a shared server machine within an enterprise, or in a hosted environment 
such as Amazon Web Services or Microsoft Azure with a minimum of effort."

This is encouraging but refers to a small enterprise team preparing technical documentation, who presumably have 
access to IT skills and/or support. My guess is that this does indeed make it "as easy as it can be" and is therefore
the best starting point. But it will require more than a few hours getting up to speed, especially from a pre-release
version that is currently not visibly under active development.

Also additional work will be required for our immediate need to integrate with Zotero and JATS and eventually for 
exploratory animations. But essentially this confirms feasability.

Found via this paper and slides:

https://www.balisage.net/Proceedings//vol15/html/Kimber01/BalisageVol15-Kimber01.html

Note links for:

- print/mobile (print this to pdf file)
  * https://www.balisage.net/Proceedings//vol15/print/Kimber01/BalisageVol15-Kimber01.html
- epub
  * https://www.balisage.net/Proceedings//vol15/epub/Kimber01/BalisageVol15-Kimber01.epub
- slides and materials (start here for overview)
  * https://www.balisage.net/Proceedings//vol15/author-pkg/Kimber01/hyperdocument-management-no-ki-magic.zip
  

Main documentation here:

http://www.d4st.org/d4st-docker/index.html


The main repository includes the others as sub-modules. I have forked it here:

https://github.com/thecapitalistcycle/dita-for-small-teams

There are 7 d4st docker files here:

https://hub.docker.com/search?q=d4st&type=image

Including update of DITA OT five months ago.

Not checked GitLab carefully for related projects.

Also need to check DITA community.

## GitLab

Most frightening aspect looks like use of dockerized GitLab Community Edition.

This is major. I had in mind just being GitLab users. Local version needed for private stuff in enterprises but I 
thought it would require extensive system administration that can be avoided for open publishing.

But project does seem to be actively maintained and popular:

https://github.com/sameersbn/docker-gitlab

## oXygen

Uses web author version. This suits orientation to Windows/Mac technical writers.

Our orientation is for most writing in LwDITA markdown with licensed oXygen editor only needed for maps and final editing by an editor more familiar with DITA. Not sure how to handle this. Will also want JATS.

https://github.com/sameersbn/docker-gitlab

