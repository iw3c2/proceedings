# Introduction

This page is to collect the requirements for a new-style proceedings of our conferences. The requirements separate what we should offer per individual publication from what we should offer for the proceedings as a whole. These requirements, when final, should govern our development, our choice of external tools, etc.

For each category, the requirements are divided into three categories:

1. **“Absolute Requirement”**: means that the feature is essential; it is a *must*, i.e., missing this item is a deal breaker
2. **“Strong Requirement”**: means that, if we have several possible solutions, availability of this item may be a reason to choose one or the other solution
3. **“Nice to have”**: if possible, we should have this but only if both (1) and (2) are fulfilled.

Note that we may do actually more than what is listed here (e.g., to provide animated tools for data presentations, provide links to similar papers, etc. This list should, however, restrain itself to what is realistic to deliver within our timeframe, time and energy restrictions. If more is done, that is cherry on the cake! (If you want to get inspired, look at the [separate page on examples](examples.md), in particular the possibilities offered by the [Utopia reader](http://utopiadocs.com/demo/) although, alas!, that is based on PDF…)

Some of the items below, e.g., availability of keynote materials or presentation slides, is the responsibility of the respective proceedings‘ chair for the conference. The list below is based on the assumption that those materials *are* available. 

There is a reference to alternate proceedings, e.g., proceedings of workshops. We should note that while a number of workshops may choose to be part of the WWW proceedings (and we should be open to that) others may decide to go their own ways for whatever reasons. At this moment we should keep to the policy of leaving this door open for them.

As publication metadata are a strong requirement, and are also necessary for issuing conference programs and webapps, we should try to integrate the generation of proceedings, programs and apps in a common workflow. To do so, exposing the conference metadata using the [Semantic Web Conference vocabulary](http://data.semanticweb.org/ns/swc/swc_2009-05-09.html) can be of interest.

---

# Individual publications

These requirements are both for the bona fide proceedings papers, i.e., for the refereed papers, but also for, e.g., the separate proceedings of a workshop if published on our web site (i.e., the quality requirements should not be more lax for non-refereed papers).

## Absolute Requirement
* Article in (valid) HTML5 with no dangling links as for datasets, external media, etc.
	* Extra resources like extra CSS or JavaScript, as well as embedded materials like figures, images, Web Fonts, etc, *must* be stored locally on the system alongside the paper itself. The goal is that the papers must stay readable as submitted for perpetuity
* Easy access to the usual metadata (title, authors, DOI, authors' ORCID, etc) in BibTeX
* Access to offline formats in PDF (following the PDF format of ACM) and EPUB
* Access to the presentation slides
* One-click addition of the reference to Twitter, Facebook, Pocket, etc,

## Strong Requirement
* Easy downloads of the usual metadata in RDF (serialized in Turtle and/or JSON-LD)
* "Social" features, e.g., commenting on the papers with answers (authors should be automatically notified of traffic)
* Separate list, with suitable on-line references, of all the supplementary materials like videos, data sets, etc.
* Datasets, media, etc, referred from the paper should also be stored, if possible, locally to ensure long term preservation (recognizing that there may be practical limitations as for the amount of data the IW3C2 can store, or legal issues that may make that type of storage impossible)


## Nice to have
* Table of Contents and/or references accessible while reading a paper, without leaving the current interface
* Better reference list handling, e.g.,
	* Details of a reference entry should appear as popup when hovering on the reference in the paper
	* Reference entries should also be available as data (RDF, BiBTeX) for easy incorporation to the researcher's workflow
* Connector to systems like Zotero or Mendeley
* Direct annotation of the paper instead of traditional commenting (e.g., incorporation with Hypothes.is facilities)
* Local storage of supplementary materials, presentation slides, etc, to ensure a long-term preservation
	* Supplementary materials may *not* be available for local storage for a variety of reasons (legal, practical, etc); this item is on *offering* this facility to authors, rather than requirements.

# Proceedings as a whole

The main requirements for individual articles are also valid for the proceedings as a whole, considered as a single publication by itself. This section lists only the extra facilities.

## Absolute Requirement
* Search on the papers by authors, titles, keywords
* Inclusion of keynote presentations, provided we get an authorization of the speakers

## Strong Requirement
* Inclusion, if available, of the materials of the alternate tracks (industrial, developers', etc.)
	* Note that, in some cases, these tracks do not have papers in the traditional sense, in which case the requirements for individual publications should be "downgraded" accordingly. 

## Nice to have
* Full text search over the text of the papers
* Semantic search (SPARQL interface?) over the publications' metadata  
* Inclusion (if possible) additional media on the conference (photos, videos, etc.) all under the roof of the proceedings

