# Foundries.io Style

This repository contains an implementation of the FoundriesFactory™ Platform style guide.
Use this with the [Vale](https://github.com/errata-ai/vale)([LICENSE](https://github.com/errata-ai/vale/blob/v2/LICENSE)) linter.

The Style guide itself also lives in the repo.

Installing from releases will also pull in the styles:

* [write-good](https://github.com/errata-ai/write-good); general good practices for writing in English
* [alex](https://github.com/errata-ai/alex); checks for insensitive or inappropriate language

## Overview

Vale is a linter for text; it checks a document for following a *style*.
In (and out) of Vale, a style is a set of rules, such as our Style Guide.
We can define these rules in a YAML file for Vale to use,
Rules go into a folder placed within the directory pointed to by `StylesPath`:

`Styles/Fio-docs/<rule_name>.yml`

`StylePath`, styles to use, and other options go into the configuration file.
This can be `_vale.ini` or `.vale.ini`, and Vale will look first in the current
directory, and then in the users home directory.

* [Writing styles for Vale](https://vale.sh/docs/topics/styles/)
* [Installing Vale](https://vale.sh/docs/vale-cli/installation/)
* [Setting up and Configuring Vale](https://vale.sh/docs/vale-cli/structure/)

Vale has [integrations](https://vale.sh/docs/integrations/guide/) with common editors/IDEs.

## Rule Implementation

The following rules were extracted from the style guide.
Below is their status as of 2026 August:

| Rule                          | Added   | File                     | Type     |
| :---:                         | :---:   | :---:                    | :---:    |
| Preset tense                  | no      | --                       | skill    |
| Active voice                  | no      | --                       | both     |
| American Spelling             | no      | --                       | both     |
| Em dash                       | yes     | `em-dash.yml`            | linter   |
| En dash                       | yes     | `en-dash.yml`            | linter   |
| Em dash tic                   | no      | --                       | skill    |
| Excessive commas              | no      | --                       | both     |
| Oxford comma                  | yes     | `oxford-comma.yml`       | linter   |
| Acronyms                      | yes     | `expand-acronyms.yml`    | linter   |
| Branding and Names            | yes     | `branding-and-names.yml` | linter   |
| Trademarks                    | partial | multiple                 | linter   |
| Nosuchthing as secure         | parital | `security-focused.yml`   | both     |
| No gurantees                  | yes     | `help-not-ensure.yml`    | linter   |
| No duplicate headers          | no      | --                       | linter   |
| Min repeated content          | no      | --                       | both     |
| Image descriptors             | no      | --                       | both     |
| Ambiguous language            | yes     | `ambigous-language.yml`  | linter   |
| Matching tone/voice           | no      | --                       | both     |
| Avoid idioms                  | no      | --                       | both     |
| Limit metaphors               | no      | --                       | skill    |
| Avoid contractions            | yes     | `Contractions.yml`       | linter   |
| Sentence length               | partial | `sentence-length.yml`    | both     |
| Wordiness                     | no      | --                       | both     |
| Inclusive language            | yes     | `InclusiveLanguage.yml`  | linter   |
| No "click here"               | yes     | `No-click-here.yml`      | linter   |
| Excessive links               | no      | --                       | linter   |
| Attribution                   | no      | --                       | skill    |
| Avoid Humor                   | no      | --                       | skill    |
| Negative Contrastive language | no      | --                       | skill    |
| Precede list with colon       | no      | --                       | linter   |
| Limit list depth              | no      | --                       | linter   |
| Enumerate steps               | no      | --                       | skill    |
| Letter options                | no      | --                       | skill    |
| Bulleted list                 | no      | --                       | skill    |
| List punctuation              | no      | --                       | skill    |
| Table rules                   | no      | --                       | skill    |
| Header Capitalization         | yes     | `Header-cap.yml`         | linter   |
| cli option bullet list        | no      | --                       | skill    |
| host example format           | no      | --                       | skill    |
| device example format         | no      | --                       | skill    |
| root example format           | no      | --                       | skill    |
| Pygments syntax choice        | no      | --                       | skill    |
| italics usage                 | no      | --                       | both     |
| Bold usage                    | no      | --                       | both     |
| tip admonition                | no      | --                       | skill    |
| warning admonition            | no      | --                       | skill    |
| note admonition               | no      | --                       | skill    |
| Semantic line breaks          | no      | --                       | both     |
| Line Column Length            | no      | --                       | both     |
| Dictionary                    | no      | --                       | resource |
| Agent Glossary                | no      | --                       | resource |

**Rule** states the guideline in less than four words;
consult the style guide for explanations.

**Added** summarizes their implementation status.

**File** indicates file name.
Linter rules are found `Fio-docs/`.

**Type** indicates if it is a linter rule,
Agent skill file, both, or a shared resource.
Agent skills are either "linter-like", meant to assist with editing existing content,
or content generation skills.
The resource type are for human, linter, and Agent, and serve to provide a vocabulary.
