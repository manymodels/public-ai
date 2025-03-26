---
title: Atlas of Knowledge
layout: page
description: An atlas of knowledge and catalog of sources needed to ground public interest AI.
---

## OMN: Manifesto for an open civilization

Collective knowledge defines our civilization. 
Our knowledge of the past, awareness of the present, and capacity to learn from ongoing discoveries, must be cherished.  
Libraries exist to serve this purpose, and are currently beloved and strong in most parts of the world.  
But they are also inherently vulnerable, and throughout history are regularly attacked and destroyed. 

The rise of strong AI greatly increases the need for organizing public knowledge of the world,  
while at the same time amplifying incentives to manipulate it, and providing new tools to alter sources at scale. 

[We need a planetary library](https://github.com/manymodels/public-ai/blob/main/atlas/omnifesto.md) that preserves the tenets of public librarianship: preservation, access, privacy.  A good library is:

- **publicly accessible**, ensuring all have access to some form of the societal record
- **publicly curatable**, open to contribution, organization, and annotation by a global community
- **robust to manipulation**, with attention to provenance and fingerprinting
- **robust to destruction**, with a widely distributed catalog and network of backups

We must learn from the successes of the great libraries of the past, and the challenges they faced.  
We must make it easier to preserve and federate public knowledge than to manipulate and destroy it.
And we must help those building the planetary library of tomorrow find support from all corners, 
and overcome obstacles placed in their way by those who do not want such institutions to exist.

[Sign up to get involved](https://docs.google.com/forms/d/1_HKkfLimn_krqkNdMHgo1we7iXmfJDDlkHB_JHXX08s/){:target="_blank" rel="noopener" class="button"}

## Omnipedia: Compiling a Atlas of knowledge

A proper atlas should include a **map** of past, present, and future works; a **catalog** of sources; and a knowledge **graph** of entities, claims, and ideas in those works.

1. Libraries today focus on holding classical works and artefacts, from past and present: mainly books, articles, and other monographs. But they have a hard time visualizing what may be missing; the [most comprehensive map of all ISBNs](http://phiresky.github.io/blog/2025/visualizing-all-books-in-isbn-space/) and where they are held was produced by an independent designer in response to a bounty held by a pirate library.
Moreover most knowledge today is in webpages online, held by few libraries (save for the Internet Archive, which receives almost no public support).  
Fully capturing the present requires engaging in work like Common Crawl, search indexing, and the Wayback Machine, and visualizing the gaps there as well.
Finally, most knowledge of tomorrow will pass through AI systems, produced and varied at much higher rates, greatly changing the current mode of single-author works.  
Capturing the provenance of future works starts with their early drafts and iterations.

2. To know what knowledge need to be preserved, we need a catalog of published works.  
At this point the lack of an open catalog is a critical failure point in library infrastructure.
The best current global catalog, WorldCat, is not open data. It cannot be easily accessed to clean up, visualize, or annotate it at scale. 
Most participating libraries (who provide the data in the first place) want an open global catalog, and have asked for one for years.  
And there is no mechanism to include popular or essential works that are not held in a member library's collection; for instance resources
hosted by Hugging Face or posted to WikiSource do not appear.

3. The most popular public knowledge graph is Wikidata, with 100 million entities and an average of 15 statements about each.  Much larger graphs exist within companies such as major search engines, 
but none intend to make them public, and the private graphs are often stored in a way that entangles the information with trade secrets about how the companies store and process knowledge.
Wikidata needs a new backend if it is to scale up; we have run some benchmarks that suggest that it can scale by another factor of 10 
with available open source backends, even without further optimization, which would allow it to scale to the size of the global library catalog.


## Concordance: Designing a planetary library

A truly planetary library is one that draws on resource from everywhere, is available for everyone, and can be carried with you in a pocket.  
It should be designed to be maintained and distributed through pluricentral community networks, not through proprietary gatekeepers with conflicts of interest that inevitably restrict access.  
Some of the greatest knowledge projects of our time (UniProt, Wikipedia, OpenStreetMap) have been built in just this way.
And it should be an integral part of providing auditable, transparent AI systems, grounded to verifiable knowledge.

There are people all over the world working to make this a reality, and modern AI tools greatly reduce the barriers to maintenance and completion of the most pressing tasks.  
However they also create new potential vulnerabilities that need to be addressed.

The Public AI Network hosts a Slack community which connects together experts from leading public AI projects, libraries, and civil society groups. 
We have an #omnipedia channel for discussing how to compile an initial Atlas.  
And we also host a regular [seminar series](https://publicai.network/seminar) that shares insights from people working in the field.   


## Getting involved

This is a public, collaborative effort.  There are a range of projects at different levels of [readiness](https://en.wikipedia.org/wiki/Technology_readiness_level) being worked on, that could use extra help.

* Wikidata: [Scaling Wikidata](https://www.wikidata.org/wiki/Wikidata:Scaling_Wikidata/Benchmarking)[7] – Repeating the benchmarking to date with a database 10x and 100x larger, on machines of different sizes.  Working with the QLever team to help them scale performance for this use case.
* Wikidata: [Sum of all GLAMs](https://www.wikidata.org/wiki/Wikidata:WikiProject_sum_of_all_paintings)[6] – compiling metadata about all significant library and museum items, and their digitization status, to help local archivists and community members complete the epic task of finishing digitizing our cultural heritage. Started in earnest with images of paintings and monuments.
* Sources: [Shared Citations](https://meta.wikimedia.org/wiki/WikiCite/Shared_Citations)[5] – Implementing a simple subset of a well-scoped project to harmonize citations, starting with those from Wikipedia articles to their sources, in a way that makes it easy to gather statistics of use, and annotate cites with their reliability in context.
* Provenance: Implementing a standard way to add a content hash[3] or other marker to ease future authentication that a preserved document has not been altered, for all works in the library
* Backups: Implementing a visualization of the rarity of works in the library[7], and where they are held, based on existing catalog information.  Building on this excellent [visualization of all ISBNs](https://phiresky.github.io/blog/2025/visualizing-all-books-in-isbn-space/). 
* Reference works: [Building a bigger wiki](https://github.com/wikius/omnipedia).[5] – an AI project to build tools for automating curation and review at scale, to keep pace with the improvements in producing summaries and sourced synthesis about a topic.
* Concordance Catalog: OpenCat[5] – Implementing a global open-data alternative to WorldCat that all GLAM institutions can contribute their metadata to, if they want it to be freely accessible to all. Working so far with a network of librarians in the US and Europe.
* [Concordance](https://docs.google.com/document/d/1DCJdStQJISEzSNu9H2vnDLaqx_5_NWjWpPnJvUsvn88/) Library:[3] Amplifying the work of the Internet Archive across more institutions and jurisdictions, to collect and preserve copies of everything in the global catalog.
* Concordance Crawl: [FineWeb2](https://github.com/huggingface/fineweb-2) does an excellent job of adding curation, clustering, and linguistic diversity to CommonCrawl; this would combine that work with the complementary work of the Wayback Machine (to gather more comprehensive snapshots of many sites) and Common Corpus (to identify the largest freely-licensed subset).
* Fully open frontier models: Training the best possible model on sources grouped by how freely they are licensed. In progress by Pleias and a few others, needs support. 
* .. _[(add yours!)](https://docs.google.com/forms/d/1_HKkfLimn_krqkNdMHgo1we7iXmfJDDlkHB_JHXX08s/edit)_

 
## Events
- April 16, 2025:  Workshop @Berkman-Klein Center, Cambridge MA
- March 26, 2025:  Cosmos Demo Day [slides](https://docs.google.com/presentation/d/1stAGX3S7OV78N8IShyDuHmfBvUzYOM9I0UQcxjMuMB8/) (sponsor of this work!)
: A new role for libraries in the AI Age @Utah library directors meeting
- March 15, 2025:  Talk + office hours @Funding the Commons, SF
- March 9, 2025:   Wikipedia + AI @SXSW, Austin
- February 12-15, 2025: [AI Action II](https://docs.google.com/document/d/1IyP2jGob6Zxp1V7jjN1Ax--r45FHGYBgDhK31eoMNVU/edit?tab=t.0){:target="_blank" rel="noopener"} on the future of libraries, at Chateau du Fey in Joigny, France
- February 11, 2025: [Public AI Congress](https://lu.ma/5h2x0n33){:target="_blank" rel="noopener"} and Public AI House at AI Action Summit in Paris, France
- October 2, 2024: [Designing Public AI](https://economicsecurityproject.org/news/blueprint-to-build-public-ai/){:target="_blank" rel="noopener"} at the Rockefeller Foundation, DC
- August 13-14, 2024: [Building a More Public AI Ecosystem](https://publicai.us){:target="_blank" rel="noopener"} at the Library of Congress

## Acknowledgements

### Related work
* Internet Archive (the first truly global digital library)
** [INTERNETARCHIVE.BAK](https://wiki.archiveteam.org/index.php/INTERNETARCHIVE.BAK/nominations) (a crowdsourced effort to back up IA)
* [Common Crawl](https://commoncrawl.org/web-graphs) (constant crawl)
* [Common Voice](https://commonvoice.mozilla.org/en/languages) (voice model production in 130+ langs, Mozilla)
* Common Corpus (by Pleias, training fully free models)
* Current.ai (identifying gaps in the public AI stack)
* Library of Congress and British Library (the largest attempts to do this for physical works, for their countries)
* Digital Public Goods [registry](https://www.digitalpublicgoods.net/registry) [tiny but valiant, UN support]
* https://docs.google.com/document/d/1DCJdStQJISEzSNu9H2vnDLaqx_5_NWjWpPnJvUsvn88/edit?tab=t.0#heading=h.de7djlc2s6ho
* [Data](https://www.reddit.com/r/DataHoarder/comments/h02jl4/lets_say_you_wanted_to_back_up_the_internet/) [Hoarders](https://www.reddit.com/r/DataHoarder/comments/l4rj44/how_to_back_up_download_the_library_of_congress/) and cottage archivists
* Libraries as outlets for Public AI (proposal with US state libraries and LOC)
* [Plurality](https://www.plurality.net/) (an example of massively multiplayer curation of a single volume)
* Efforts by IA, 🤗 , and other libraries to [Let the Robots Read](https://docs.google.com/document/d/1k614XlIcdWxJ0gFyuC0ovlNI5XMd-54P6ATeRPo2ORw/)
* The [Data Rescue Project](https://docs.google.com/document/d/15ZRxHqbhGDHCXo7Hqi_Vcy4Q50ZItLblIFaY3s7LBLw/) (global and national)
* Chapter draft "_NERFED: The dismantling of America's libraries and global stewardship of information_" via BW
* WP specific:  [ML modeling](https://meta.wikimedia.org/wiki/User:Isaac_(WMF)/ML_modeling_at_Wikimedia), [AI dataset recs](https://meta.wikimedia.org/wiki/User:Isaac_(WMF)/AI_Datasets) and [data gaps](https://meta.wikimedia.org/wiki/User:Isaac_(WMF)/Content_tagging/Data_gaps)

## License
The work in this repository is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/){:target="_blank" rel="noopener"}.
