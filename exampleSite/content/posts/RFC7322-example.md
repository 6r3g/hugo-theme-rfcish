---
title: "RFC 7322 - RFC Style Guide"
author: H. Flanagan, S. Ginoza
date: 2014-09-01
categories: Showcase
series: Lorem
tags: ["rfc7322", "rfc", "style" ]
toc: true
---
  
# Abstract

This document describes the fundamental and unique style conventions
and editorial policies currently in use for the RFC Series.  It
captures the RFC Editor's basic requirements and offers guidance
regarding the style and structure of an RFC.  Additional guidance is
captured on a website that reflects the experimental nature of that
guidance and prepares it for future inclusion in the RFC Style Guide.
This document obsoletes RFC 2223, "Instructions to RFC Authors".

# Status of This Memo

This document is not an Internet Standards Track specification; it is
published for informational purposes.

This document is a product of the Internet Architecture Board (IAB)
and represents information that the IAB has deemed valuable to
provide for permanent record.  It represents the consensus of the
Internet Architecture Board (IAB).  Documents approved for
publication by the IAB are not a candidate for any level of Internet
Standard; see Section 2 of RFC 5741.

Information about the current status of this document, any errata,
and how to provide feedback on it may be obtained at
http://www.rfc-editor.org/info/rfc7322.

# Copyright Notice

Copyright (c) 2014 IETF Trust and the persons identified as the
document authors.  All rights reserved.

This document is subject to BCP 78 and the IETF Trust's Legal
Provisions Relating to IETF Documents
(http://trustee.ietf.org/license-info) in effect on the date of
publication of this document.  Please review these documents
carefully, as they describe your rights and restrictions with respect
to this document.

## Introduction

The ultimate goal of the RFC publication process is to produce
documents that are readable, clear, consistent, and reasonably
uniform.  The basic formatting conventions for RFCs were established
in the 1970s by the original RFC Editor, Jon Postel.  This document
describes the fundamental and unique style conventions and editorial
policies currently in use for the RFC Series [RFC4844].  It is
intended as a stable, infrequently updated reference for authors,
editors, and reviewers.

The RFC Editor also maintains a web portion of the Style Guide (see
Appendix A.3) that describes issues as they are raised and indicates
how the RFC Editor intends to address them.  As new style issues
arise, the RFC Editor will first address them on the web portion of
the Style Guide [STYLE-WEB].  These topics may become part of the RFC
Style Guide when it is revised.

The world of technical publishing has generally accepted rules for
grammar, punctuation, capitalization, sentence length and complexity,
parallelism, etc.  The RFC Editor generally follows these accepted
rules as defined by the Chicago Manual of Style (CMOS) [CMOS], with a
few important exceptions to avoid ambiguity in complex technical
prose and to handle mixtures of text and computer languages, or to
preserve historical formatting rules.  This document presents these
exceptions as applied or recommended by the RFC Editor.

All RFCs begin as Internet-Drafts (also referred to as I-Ds), and a
well-written and properly constructed Internet-Draft [ID-GUIDE]
provides a strong basis for a good RFC.  The RFC Editor accepts
Internet-Drafts from specified streams for publication [RFC4844] and
applies the rules and guidelines for the RFC Series during the
editorial process.

## RFC Editor's Philosophy

Authors may find it helpful to understand the RFC Editor's goals during the publication process, namely to:
- Prepare the document according to RFC style and format.
- Make the document as clear, consistent, and readable aspossible.
- Correct larger content/clarity issues; flag any unclear passages for author review.
- Fix inconsistencies (e.g., terms that appear in various forms, text that appears multiple times, or inconsistent capitalization).

We strive for consistency within:
a. the document,
b. a cluster of documents [CLUSTER], and
c. the series of RFCs on the subject matter.

The editorial process of the RFC Editor is not an additional
technical review of the document.  Where the RFC Editor may suggest
changes in wording for clarity and readability, it is up to the
author, working group, or stream-approving body to determine whether
the changes have an impact on the technical meaning of the document
[RFC4844].  If the original wording is a more accurate representation
of the technical content being described in the document, it takes
precedence over editorial conventions.

The activity of editing sometimes creates a tension between author
and editor.  The RFC Editor attempts to minimize this conflict for
RFC publication while continually striving to produce a uniformly
excellent document series.  The RFC Editor refers to this fundamental
tension as "editorial balance," and maintaining this balance is a
continuing concern for the RFC Editor.  There is a prime directive
that must rule over grammatical conventions: do not change the
intended meaning of the text.

If the RFC Editor cannot edit a document without serious risk of
altering the meaning, it may be returned to the stream-approving body
for review.  See Appendix A.2 for more information.

## RFC Style Conventions

This Style Guide does not use terminology as defined in RFC 2119
[BCP14].  In this document, lowercase use of "must" and "should"
indicates changes the RFC Editor will make automatically to conform
with this Style Guide versus those that may be questioned if not
applied.  The lowercase "must" indicates those changes that will be
applied automatically and are not at the discretion of the authors.
The lowercase "should" indicates the RFC Editor's recommended use,
but conformance with the recommendations is not required; the RFC
Editor may question whether the guidance may be applied.

###  Language

The RFC publication language is English.  Spelling may be either
American or British, as long as an individual document is internally
consistent.  Where both American and British English spelling are
used within a document or cluster of documents, the text will be
modified to be consistent with American English spelling.

### Punctuation

*  No overstriking (or underlining) is allowed.
*  When a sentence ended by a period is immediately followed by
another sentence, there must be two blank spaces after the period.
*  A comma is used before the last item of a series, e.g.,
"TCP service is reliable, ordered, and full duplex"
*  When quoting literal text, punctuation is placed outside quotation
marks, e.g.,

Search for the string "Error Found".

When quoting general text, such as general text from another RFC,
punctuation may be included within the quotation marks, e.g.,

RFC 4844 indicates that "RFCs are available free of charge to
anyone via the Internet."

Quotation marks are not necessary when text is formatted as a
block quotation.

###  DNS Names and URIs

DNS names, whether or not in URIs, that are used as generic examples
in RFCs should use the particular examples defined in "Reserved Top
Level DNS Names" [BCP32], to avoid accidental conflicts.

Angle brackets are strongly recommended around URIs [STD66], e.g.,  
<http://example.com/>

###  Capitalization

*  Capitalization must be consistent within the document and ideally
should be consistent with related RFCs.  Refer to the online table
of decisions on consistent usage of terms in RFCs [TERMS].

*  Per CMOS guidelines, the major words in RFC titles and section
titles should be capitalized (this is sometimes called "title
case").  Typically, all words in a title will be capitalized,
except for internal articles, prepositions, and conjunctions.

*  Section titles that are in sentence form will follow typical
sentence capitalization.

*  Titles of figures may be in sentence form or use title case.

###  Citations

*  References and citations must match.  That is, there must be a
reference for each citation used, and vice versa.

*  Citations must be enclosed in square brackets (e.g., "[CITE1]").

*  A citation/reference tag must not contain spaces.

Example: "[RFC2119]" rather than "[RFC 2119]"

However, the proper textual naming of an RFC contains a space.

Example: "See RFC 2119 [BCP14] for more information."

*  Cross-references within the body of the memo and to other RFCs
must use section numbers rather than page numbers, as pagination
may change per format and device.

###  Abbreviation Rules

Abbreviations should be expanded in document titles and upon first
use in the document.  The full expansion of the text should be
followed by the abbreviation itself in parentheses.  The exception is
an abbreviation that is so common that the readership of RFCs can be
expected to recognize it immediately; examples include (but are not
limited to) TCP, IP, SNMP, and HTTP.  The online list of
abbreviations [ABBR] provides guidance.  Some cases are marginal, and
the RFC Editor will make the final judgment, weighing obscurity
against complexity.

Note: The online list of abbreviations is not exhaustive or
definitive.  It is a list of abbreviations appearing in RFCs and
sometimes reflects discussions with authors, Working Group Chairs,
and/or Area Directors (ADs).  Note that some abbreviations have
multiple expansions.  Additionally, this list includes some terms
that look like abbreviations but that are actually fixed names for
things and hence cannot and should not be expanded.  These are
noted as "No Expansion".

## Structure of an RFC

A published RFC will largely contain the elements in the following
list.  Some of these sections are required, as noted.  Those sections
marked with "*" will be supplied by the RFC Editor during the
editorial process when necessary.  Sections are allowed to contain
nothing but subsections.  The rules for each of these elements are
described in more detail below.

...