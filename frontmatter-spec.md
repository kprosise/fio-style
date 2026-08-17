---
title: Documentation Front Matter Specification
description: Overview of metadata to add to the documentation for foundries projects
type: page
doc-category: informational
authors: kprosise@quicinc.com
last-edited: 2026–08–24
license: CC-BY-4.0
access: public
references: self
keywords: documentation front-matter
---

# Documentation Front Matter Specification

## Purpose of Foundries Documentation Front Matter

By providing the definition and relation of a document page, the pages can be parsed agnostic from
markup renderer.

## Usage of Front Matter

## Specification

```yaml
title:
description:
type:
doc-category:
authors:
last-edited:
license:
access:
references:
keywords:
relations:
    prev:
    next:
    parent:
```

| Field          | Purpose                    | Values                                         | Required |
| ---            | ---                        | ---                                            | ---      |
| `title`        | used in place of header    | string                                         | no       |
| `description`  | summary/purpose            | string                                         | no       |
| `type`         | Resource type              | `page`, `config`,`fragment`,`data`, `template` | yes      |
| `doc-category` | type of doc                | `informational`,`instructional`,`record`       | no       |
| `authors`      | Creators/contributors      | names or emails, include Agent id when used    | yes      |
| `last-edited`  | freshness indicator        | ISO 8601 date format                           | no       |
| `license`      | Use and distribution       | SPDX license identifier or `closed`            | yes      |
| `access`       | view rights                | `public`, `internal`, CCI level                | no       |
| `references`   | source of truth            | URL, ISBN, path, or `self`                     | yes      |
| `keywords`     | findability/sorting        | terms with a glossary/dictionary entry         | no       |
| `relations`    | TOC alternative            | --                                             | no       |
| `prev`         | previous page/document     | path, `title`, `id`, URL                       | no       |
| `next`         | next page/document         | path,`title`, `id`, URL                        | no       |
| `parent`       | if part of larger document | path, `title`, `id`, URL                       | no       |

### Field Values

#### Title and Description

`title` can be used in place of the header to represent the name of the document.

Description is a 1–3 sentence summary of the document.

#### Type and Doc-Category

`type` describes the nature of the documentation file:

- `page`: Contains the main content or a series of `includes` of `fragment` content
- `fragment`: parts of a page, such as those used for shared content or modular content
- `data`: tables/csv files, lists, and other data
- `template`: Markup template.

`doc-category` describes the basic nature of the documentation:

- `informational`: Contains technical information, such as a Reference Manual, API documentation or
  FAQ
- `instructional`: Guides the reader through a series of steps, such as a Getting Started guide or
  Tutorial.
- `record`: A list like entry, such as a glossary, or a record of change, such as a changelog or
  release notes.

#### Authors and Last Edited

`authors` records who created or contributed to the file. If an AI agent was used, please provide
information to identify it.

`last-edited` is the ISO 8601 date format that the document was last updated.

#### License and Access

`license` uses SPDX license identifier for any Open Source licenses in use.
All documents need to include their licenses/usage rights.
If closed/non-public, please use `closed`
license.
For documentation, this is often  `CC-BY-4.0`, for "Creative Commons Attribution International".

`access`, when used, should be in agreement with the license.
Values can be `public`, `internal` for any document not to be shared externally, or the Company's
CCI level indicator.

#### References and Keywords

`references` provide where the source of truth/knowledge is.
This can be a URL, such as to a code repository, ISBN if printed material or a file path.
Use `self` if the page is to be the primary source.
The goal is for information to be verifiable.
The source should **not** be generated content.
This field is especially important when working with an Agent; instruct them to provide all
references.

`keywords` are to improve chances of the document showing up in search results or inclusion in an
index.
Any term used as a keyword must appear in a glossary or dictionary used by the project,
unless they appear in the document title/top header.

#### Relations

Relations are used as an alternative to a Table of Contents.
If both are available, precedence is left to the builder/user.

- `prev` and `next` provide the current page's location in a sequence.
- `parent` has a depth of 1 from the page. Used for sections/subsections.
