# Foundries Style and Communication Guide

## Introduction

Welcome to our style and communication guide.
This guide covers guidelines, rules, and suggestions related to technical communication.

This is a living document and subject to change.
Reach out to the technical writing team if you have any questions, or have feedback.

## General Style

This section covers all communication and is not limited to public documentation.
Case specific guidelines, can be found under *Document Types and Specifics.*

### Tense and Voice

Try to keep documentation and instructional in the
[present tense](https://learnenglish.britishcouncil.org/grammar/english-grammar-reference/present-tense).
Speak to the state of something as it currently is, e.g., “with the disk now partitioned”.
Future Tense generally uses the verb “will” and is also acceptable.

In most cases, use the [active voice](https://www.grammarly.com/blog/active-vs-passive-voice/).
Git commits, for example, always use the active voice as they are written in the imperative, e.g.,
“Fix typos in the Getting Started Guide”.
The Reference Manual and the Glossary may use passive.

### Grammar, Punctuation, and Spelling

For differences between American and British English, use American spelling.
The exception is material targeting a specific locale where American spelling would be out of place.

#### Dashes and Hyphens

This section covers the difference between hyphens, en dashes, and em dashes.

**Hyphens** `-` can be used when:

- joining two words to form a compound word;  *back-up*
- Spelling out a number; *eighty-nine*
- Justifying words; this is usually done automatically..

**En dashes** `–` are used to…

- Numerical Dates; *2022–12–21*
- Numerical Ranges; *It may take between 20–60 minutes for your build to finish*

**Em dashes** `—` are used to…

- draw attention where one may otherwise use parenthesis, commas, semicolons or colons

This may be in the middle of a sentence—the most common use—or at the end followed by a period.
Spacing or lack of around the Em dash is style oriented-blog posts and the like can use the authors preference.
In documentation, buffer the em dash facing outwards, but leave connected to the statement you are drawing attention towards.

> [!IMPORTANT]
> A common "tic" in AI generated documentation is the overuse of em-dashes.
> To avoid blocking all use of the em-dash, limit the sentence word count to around 25 words.
> Note that there are some cases, such as writing reference material,
> where avoiding em-dashes is appropriate.

#### Commas

Limit the number of commas used in a sentence.
Checking for excessive use of commas can also help identify run on sentences.
They can also read as “bland” and non-descriptive.
Ask yourself if an em dash, semi colon, or other punctuation better separates ideas.

To aid in clarity, as well as reading rhythm, use the **oxford comma**.
The oxford comma is placed directly after the next to last term in a list,
before the coordinating conjunction (such as *and*,*or, *and *nor*).

- Wrong: "Next you will write, build and install the package”
- Correct: "Next, you will write, build,and install the package".

#### Abbreviations

| Example of | Incorrect | Correct |
| --- | --- | --- |
| Initialism | IoT (Internet of Things) | Internet of Things (IoT) |
| Acronym | GIF (Graphics Interchange Format) | Graphics Interchange Format (GIF) |
| Short Form | Dist | Distro |

An acronym or initialism is **preceded** by the expanded form, for the first occurrence in a resource.
The letters that make up the abbreviation should be capitalized.

- Shortened words do not need to be presented in full form, but limit to ones the audience is familiar with.
- Months and days of the week should **not** be shortened.

If a project or company uses a shortened form, use that instead of an abbreviation.
For example, Visual Studio Code is shortened to VS Code, not "VSC".

#### Names and Branding

When mentioning projects, businesses, and services, check that you are using the correct capitalization and spacing:

| Incorrect  | Correct |
| --- | --- |
| github | GitHub |
| Open Embedded | OpenEmbedded |
| Javascript | JavaScript |

When using anything which is **trademarked or copyrighted**,
the **first occurrence** on the page usually utilizes the appropriate symbol.
The general exception being if it is in a title or box content.
In that case include it in the next usage.

Some specifics:

- Full company name should be used; as in **Foundries.io.**
- **F**oundries**F**actory™  Platform
- **L**inux **m**icro**P**latform, **LmP**
- **a**ktualizr**-l**ite
- **F**ioctl® utility
- **O**pen **S**ource; capitalize the first letters.
  Do not abbreviate as to avoid confusion with Operating System.
- Images has multiple relevant definitions. When context does not make it clear, qualify: **system image**, **graphical image**, **Docker image**.
- **G**o programming language: Capitalize the first letter, this holds true for most programming languages.
- **Docker**:
  - **D**ocker** C**ompose, **C**ompose
  - **Dockerfile**
  - Docker **D**esktop
  - Docker **H**ub
  - Docker **c**ontainer.

### Word Choice, SEO, and AIO

#### Statements on Security

Avoid stating that something is secure, securable, or the act of securing as an absolute.
Approach this pedantically;
there is no such thing as *totally secure*.
Instead, use terms such as  *protecting* or *security-focused*.

#### Search Engine Optimization

- “Search Engine Optimization (SEO) is the process of improving the quality and quantity of website traffic to a website or a web page from search engines.
  SEO targets unpaid traffic rather than direct traffic or paid traffic”. [source: Wikipedia]

##### Overview of SEO

[Foundries.io](http://Foundries.io) marketing team is working with the external agency **Booyah** on all SEO related activities.

Our main SEO related tasks:

1. Metadata
  - This is the main home for keyword targeting.
    It contains the most valuable placements (title tag, meta description) as well as a way for us to organize our keyword targeting and avoid internal cannibalization.

1. Interlinking
  - This is how we build the internal association web between our own pages.
    It is helpful for strengthening keyword performance on target pages by using the keyword as anchor text.
    Make sure that no internal links break if/when internal URL structure updates.

### Artificial Intelligence Optimization

Artificial Intelligence Optimization (AIO).
This is what helps content consumed by AI remain accurate and largely free of hallucinations.
The same practices make content read by a user readable and lessens misunderstandings.

#### Overview of AIO

New information should involve a person or human team so as to establish a **source of truth**.

Best practices:

- Keep content unique;
  avoid restating information available elsewhere, and reduce duplicate content.
  - It’s okay to phrase things differently for different contexts and audiences
- Organize content so that it is easy to follow and digest:
  purposeful paragraphs and subsections.
  Try to keep headers/section names unique;
  sections that share the same name are harder to quickly navigate and parse.
- Add textual context to images/video.
- Use accessibility checks/linters.
  There is a heavy overlap between accessible content and AI output.
- Stable layout:
  Put thought into how content is laid out at the start,
  and try to limit any changes.
- When working with HTML templates, try to use Semantic HTML.
- Keep content simple!
  Break apart clauses and phrases into simpler sentences.
  Try to keep sentences to 25 words or less.
- Avoid ambiguous language,
  and be mindful of metaphors and phrases that may not translate.
- Match the voice/tone with that of the surrounding content.
- Avoid Negative contrastive language, a common AI tic.

### Sentence Length

Keep the meaning clear, but be mindful of wording that does not add value.
**Maximum sentence length is 25 words.**
This is a very strong guideline.

### Inclusive and Accessible Communication

Language can have biased, discriminatory or otherwise hurtful cogitations.
Sometimes the origins or other uses are not known.
Other times it can make someone feel like an outsider or looked down on.
We must strive to do better and be better, always.

As a comprehensive list is not possible,
we will cover some specifics and general guidelines.
If you ever have questions or are unsure,
reach out to a technical writer.

#### Gender

Gender, and how it relates to concepts such as inclusivity, language, culture, and identity is complex,
and the way these concepts intersect more so.
We can follow a few guidelines that will cover most cases.

Not everyone identifies with being man or woman,
and not every culture has the same concept of gender, or see it as a binary.
To be respectful and inclusive, we can use more neutral language.
When referencing or addressing a group of people,
aim to use inclusive terms.
Example: saying “Hey everyone” or “Good morning team” rather than “Hey guys” or “Morning gents”.

Pronouns are used to reference nouns, and within this context, people.
She/her, he/him, they, everyone, are pronouns we use to refer to people.

| Type | Rather than... | Consider... |
| --- | --- | --- |
| Generic pronouns | “he/she will” or “he will” | they will |
| Group reference | “Ladies and Gentlemen”, “Guys” | “Folks”, “Team”, “Everyone” |
| Known pronouns | “Mrs. Foobar said they will be at …” | “Mrs. Foobar said she will be at“ |

When you are referring to someone generically, use the [singular they](https://en.wikipedia.org/wiki/Singular_they):

> “Ask your Sysadmin if he/she can change your password” → “Ask your Sysadmin if they can change your password”

In addition, some folks may prefer the use of [“they” as personal pronouns](https://www.mypronouns.org/they-them),
such as “Do you know if Riley is working today?
I haven’t seen **them** in the office.”

However **if you are referencing a specific person and you know the preferred pronouns, use those**.

#### Condescending, Belittling, and Ableist Language

This section discusses and provides examples of language that may be hurtful,
in order for it to be avoided.

Phrases such as “Of course”, “obviously”, or  “as everyone knows” are used frequently, so they can seem innocuous/harmless.
If the related information is not previously known to the reader, this can make content feel unwelcoming.
When writing documentation, the goal is to teach and assist.

**Never** use words such as “idiot” or ”stupid”.
In addition, there are terms related to disabilities that we should aim to avoid outside literal uses:

| Term |  Meaning and Alternative |
| --- | --- |
| blind | lacking awareness |
| lame | uncool, disappointing |
| schizophrenic | out of control, all over the place |

The above terms, as well as others, are examples [ableist language](https://hbr.org/2020/12/why-you-need-to-stop-using-these-words-and-phrases).

Belittling language can also take the form of **sexism**.
One seen in relation to technology is around the lines of “It is so easy, my Grandmother can do it”.
This is both condescending and sexist;
it may not be easy to someone, and there are grandmothers out there with doctorates in Computer Science.

#### Race, Ethnicity and Culture

This section discusses and provides examples of language that may be hurtful,
in order for it to be avoided.
It is important to remember that even though a word may have multiple contexts,
it can carry over the negativity associated with it, such has “hang”.

It is not only common slurs can be harmful.
Phrases, sayings, and terms that have become commonly used may still invoke the original, insulting usage.
Sometimes they get picked up in a different country, region, or language, where context is lost.
Examples: "Off the res", "gypsy/gyp", "uppity", [and more](https://www.businessinsider.com/offensive-phrases-that-people-still-use-2013-11#2-uppity-2).

Examples of common terms that may appear when discussing technology:

| Rather than... | Consider... |
| --- | --- |
| Master/slave | main/second |
| hang | does not respond |
| Blacklist/whitelist | blocklist/allowlist |

> Keep in mind that it is permissible to use the outdated technical terms if required,
> such as when discussing specific git branches.
> If discussing git branches in general however, use main rather than master if possible within context.

#### Word Choice for a Diverse and Global Community

Make things easier for those who do not have English as their first language.
Even for native speakers, parsing through technical information can be difficult.
Avoid creating the need to make someone look up the meaning of a word.

Additional tips:

- *Try* to avoid idioms. For example, “once in a blue moon” to mean “rarely”.
- Avoid using contractions.
- Humor and sarcasm does not always carry across cultures, languages, or communities.
  It is best to avoid sarcasm in most situations.
  If you use humor, such as in a blog or presentation, check that it does not belittle/insult anyone.

### Links, References, and Attribution

Hyperlinks:

- WC3 explains why you should not use “[click here](https://www.w3.org/QA/Tips/noClickHere)” for link text.
- If you find a paragraph or section has related links, consider grouping them under a list to make the entry easier to read.
  Links can provide useful “aside” information, but they are become distractions that overwhelm the reader.
- If referencing a source available online, provide a link to the source.

If you are directly copying from another source—including an image—make sure that it is permissible to do so.
Check for copyright information, such as a [Creative Commons usage license](https://creativecommons.org/use-remix/), or part of the Public Domain.
Be compliant and follow the attribution terms.

### Use of AI

Please follow Qualcomm guidelines for AI usage.
It is highly recommended that usage be kept to checking grammar and assisting with translation challenges.
If you feel like you must use GenAI, use skill files provided by technical writing.
Keep generated content short and easy to digest *by a human reviewer*.

### Layout and Visual Formatting

Communication is more than words.
How information is ordered, how you get attention, and how images are used, are ways that we communicate without words.
At the same time, not everyone will be able to access or parse graphics, colors, or blocks due to disabilities and differences.
Sometimes there can be so much information, it becomes overwhelming and difficult to follow—all the more common due to AI.
We need to keep things consistent and information easy to find.

This section aims to provide guides that help content be presented in a manor that is accessible.

#### Accessibility

Accessibility should not be seen as an end point; it is an objective that can always be improved.

 The following subsections aim to incorporate the recommendations of the World Wide Web Consortium’s [Web Content Accessibility Guidelines (WCAG) 2.1](https://www.w3.org/TR/WCAG21/).
 It is recommended to consult their guide.

#### Lists

From checklists and instructions to help carry out a task, to short summaries of information, lists *can* be useful aids.
For in-depth details on using lists, reference the [APA Style on Lists](https://apastyle.apa.org/style-grammar-guidelines/lists).

When providing a list you should:

- Precede it with a colon
- Use the appropriate type: letters, numbers, bullets
- Keep it short; line length and points alike
- Keep depth to one

Using a colon before beginning lets the reader knows the following points are related.
The exception is if you are beginning a section with a list.

If providing sequential steps or ranking the members, use numbers. If** order** matters, enumerate:

```restructuredtext
1. Open a terminal
2. Type sudo pacman -Syu
3. Hit enter
4. Enter your password when prompted
```

When you need to reference the members of the list, or when providing options, use letters:

```restructuredtext
To write the system image, you can:

a. use dd if=foobar.img of=/dev/mmblk0p1
b. Download and install a image writer such as...
c. Cast a spell

If you go with option a, you must be very careful to not foobar your root fs
```

> If three or less options are listed and they are short, you may keep them inline if it improves readability.

If order does not matter and you will not be needing to reference the points, you can use a bulleted list:

```restructuredtext
Prerequisites:

- Understanding of Docker
- Docker version 19.03.8 or newer
- Plenty of coffee
```

Punctuation for lists depends on content.
If each point is a complete sentence, use a period after each.
For words and phrases that are easy to read through, no punctuation is required.
For complex lists which read like a paragraph, consider using semicolons after each point,
with a period at the final one.

#### Tables

Use tables when data needs to be summarized and referenced by the reader, such as a list of supported machines.

Names should be presented in the first row, and be sorted alphabetically or numerically.
Shade alternating rows when possible.
Try to keep vertical content to a minimum and avoid the need to scroll within the table; horizontal scrolling should be avoided if possible.

Category names should be kept to columns, and entries as rows.

Where supported by markup language or framework, give tables a descriptive name/label at top.
When being done manually, choose a font smaller than the main text, and use italics.

#### Fonts

The primary Typeface is Aptos.
When not available, Roboto Flex is to be used.
Roboto Flex is used for both the website and our Documentation.

#### Headers and Sections

> [!IMPORTANT]
> Keep Headers/section names as unique/specific as possible.
> For example, rather than using "Overview", use "Overview of Headers".
>
> A documentation set where there are no repeated Headers/subsection names yields greatly improved
> search and AI consumption results.

The first header on a page should be level 1 (H1).

For subsections, do not go beyond level 4.
The example below is in ReStructuredText, but the rule applies in other instances.

```restructuredtext
Style-guide
===========

General Style
-------------

Layout and Visual Formatting
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Headers and Sections
""""""""""""""""""""
```

There should be a newline before and after section headers.

For title capitalize, follow [APA style](https://apastyle.apa.org/style-grammar-guidelines/capitalization/title-case).
In short: the first letter of all major words, and always the first word.
Minor words that are four or more letters long should be capitalized.
The use of inline code for programs or variable names is allowed.

#### Interface Examples and Code-Blocks

 When mentioning an element of a Graphical User Interface (GUI), use backticks.
 In the case of rst files, use ``:guilabel:`<element_name>` text``.
 If documenting menu navigation, provide information on where the menu can be opened from.
 For example, “top left corner menu”.
 Use “→” to indicate menu steps: “options → preferences → themes”

For Command Line Interface (CLI) examples and options, use back-ticks for inline literals.
Note that for rst, it is double back-ticks:

```restructuredtext
set variable ``FIOCTL_FACTORY``
```

Use a bulleted list to explain command options,
listing the option as a literal followed by what it does:

`foobar -r -i`

- `-r` recursively applies overly used example
- `-i` interactive, allows you to select files

For console examples, use `$ <command>` for host examples.
For embedded device environments, use `device:~$ <command>`.
For root user, use `#`.

For Sphinx/docutils, code examples use the `code-block` directive.
Sphinx uses [Pygments](https://pygments.org/languages/)for syntax highlighting.
The link above has the list of supported languages and their short name to use.
Provide the language as an argument.
It is important to note that `bash`and `shell` are for scripts.
In most cases, `console` is more appropropriate when showing a CLI example.

```restructuredtext
.. code-block:: console

   $ fioctl device show <device name>
     UUID:          a06b0bab-38be-409b-b7f8-f1125231a91e
     …

.. code-block::

.. prompt:: bash docker:~$ , auto

.. prompt:: bash u-boot#, auto
```

Code-blocks should have language set if available and appropriate, to enable highlighting.

#### Emphasis and Admonitions

When you need to draw attention to a single point,
you can apply emphasis by using italic or bold text.
You can also use an admonition.
Italics or bold work best for a word or short phrase which does not need an additional explanation.
Admonitions are for side notes and important warnings,
and can stretch over a couple sentences.

| **Attention Grabber** | **Use Case** | **Example** |
| --- | --- | --- |
| *italics* | *soft emphasis, short quotes, nuance* | You *may *need to contact your administrator first. |
| **bold** | Strong emphasis; If spoken you would possibly raise your voice, or in casual writing you may use all caps. | You must **never** consider your device 100% secure. |
| tip! | Advice which is optional to follow. | Tip: It is a good idea to make a backup before going forward. |
| ! WARNING | Calling out potentially serious consequences. | WARNING: Using `dd` will write over anything on the storage medium, make sure that you are writing to the right place and have nothing you want to keep. |
| note or info | Something to keep in mind. | Note: This document is a work in progress and is subject to change at any time |

**Admonitions** appear as boxes.
Available types and syntax will vary depending on markup language, framework, or editor.
When it comes to placement, notes and extra info should be *outside* the main context.
This can be to the side, above, or after.
Warnings should always be placed so that they are read *before* the reader would take any action which requires caution.
Tips can appear anywhere, depending on context.

**Note/Info:**

Building the image may take over 30 minutes to finish.

**Warning:**

WARNING: Geese up ahead, proceed at your own risk.

**Tip:**

#### Images, Graphics, and Video

Images should be in Portable Network Graphics (PNG) format, or webp format.

All visual content *must* include descriptive alternative text:

```restructuredtext
 .. figure:: /_static/factory/add_member.webp
    :align: center
    :alt: UI, sending Factory member invites.
```

Someone may not see the image,
such as those with a visual impairment or limited network connection.
Ask yourself if the description would help someone understand what the image portrays.
Alt text also assists with AI consumption.

---

## Document Types and Specifics

### Customer Documentation

The Foundries docs can be seen as a compendium of “books”.
Each book relates to a different need.

#### Doc types at a Glance

| **Book** | **Purpose** | **Examples** |
| --- | --- | --- |
| Getting Started | Introduces **FoundriesFactory** **basics**, key concepts and tools; From creating an account → Registering a device. | [Sign Up](https://docs.foundries.io/latest/getting-started/signup/index.html), [Installing Fioctl CLI](https://docs.foundries.io/latest/getting-started/install-fioctl/index.html) |
| Tutorials | Provides workable “A to B” examples that customers can follow along with to **become more comfortable and familiar with FoundriesFactory**. Follows Getting Started Guide. | [Working with tags](https://docs.foundries.io/88/tutorials/working-with-tags/working-with-tags.html) |
| User Guide | Covers tasks and **specific use-cases** for **customers already familiar with FoundriesFactory.** This section should enable customers to get the most out of their experience. | [Offline Updates](https://docs.foundries.io/latest/user-guide/offline-update/offline-update.html) |
| Reference Manual | Collection of information for **quick reference**, such as variable names or command options. Focuses on details, not use-cases. | [Fioconfig](https://docs.foundries.io/latest/reference-manual/ota/fioconfig.html) |
| Glossary | **Terms** and their definitions/descriptions. Abbreviations and their expansions. | [Docs Glossary](https://docs.foundries.io/latest/glossary/index.html) |
| Appendix | api/command lists, **raw information.** |  |

#### Getting Started

- Source Location: <https://github.com/foundriesio/docs/tree/master/source/getting-started>

- Purpose: To guide **any** reader from creating an account to registering a device, and where to go next.

- Tone: Friendly, helpful. Active voice

Getting Started guides are task orientated.
With new concepts and tools to learn, it is important to not overwhelm the reader.
Think of a teacher introducing a subject to their students.
Keep the steps as linear as possible, providing a clear path.
Avoid discussing edge use cases, provide links to detailed documentation sections instead.
Remember that this guide may be followed by decision makers with limited understanding or skill set.

#### Tutorials

- Source Location: <https://github.com/foundriesio/docs/tree/master/source/tutorials>

- Purpose: Covers tasks that all users will need to know how to preform.

- Tone: Similar to getting-started, exploratory and questioning, active voice

Skill oriented and complementary to the getting started guide.
Provides learning opportunities that are in-depth and focused.
Think of a mid-term university lecture;
the students understand the basics and are now ready to be guided to deeper understanding.

Where the entirety of the getting started guide can be worked though in one go,
the tutorials can be longer.
Keep them no longer than ~30 minutes.

In ReStructuredText, tutorials have the form:

```restructuredtext
.. _name-of-tutorial:

Name of Tutorial
================

High level overview of the goal, what the reader will learn

.. note::
 Estimated Time to Complete this Tutorial: N minutes

Learning Objectives
-------------------

- Objective....
- Another objective...

Prerequisites
-------------

- Completed the :ref:`a-previous-section-reference-name` section.
- Completed the :ref:`a-previous-tutorial-reference-name` tutorial.

Instructions
------------

.. toctree::
    :maxdepth: 1
    subsection-page1
    subsection-name2
    subsection-name3
    summary
```

When estimating the time it takes to complete,
it may be helpful to have someone on a different team go through it.
Consider adding minutes; if a reader completes it in less time, it can boost their confidence!

#### User Guide

- Source Location: <https://github.com/foundriesio/docs/tree/master/source/user-guide>

- Purpose: A guide through additional or advanced features.
- Similar to tutorials, but focuses on tasks that may not be relevant to every use case.

- Tone: Semi-formal, active voice.

Compared to the tutorial section,
the User Guide is self guided.
The reader consults it when they need to know how to do a special task.
Template:

```restructuredtext
.. _name-of-user-guide:

Topic/Task Name
===============

*Exceptions exist, this template provides general suggestions. Modify as seen fit.*
User guides are generally:
* *instructional*; similar to our tutorials, but with assuming familiar with basics
* *informative*; covering concepts and relaying knowledge.

Write a sentence or paragraph providing a high level overview of what this solves or discusses.

What will be accomplished, the objective.
Consider using a list.

* Provide a copy/paste template.
* Guidelines and suggestions for writing user guide pages.

Prerequisites (optional)
------------------------

- Completed the :ref:`a-previous-section-reference-name` section.
- Completed the :ref:`a-previous-tutorial-reference-name` tutorial.

Instructions/Concepts
---------------------

Add sections and subsections as you feel fit.
```

#### Reference Manual

- Source Location: <https://github.com/foundriesio/docs/tree/master/source/reference-manual>

- Purpose: Provides technical details such as envvars and explanations of components and processes.
  Think along the lines of a [Unix man page](https://en.wikipedia.org/wiki/Man_page).

- Tone: Passive voice, “matter-of-fact”.

This is where the documentation becomes focused on lower level technical details.
The reader is looking for specific information.

Use a passive voice.
Keep content technical.
We are “telling” the reader the information they need,
not “showing” them how to do something.

The following template is one form this can take, however depending on information being conveyed.

```restructuredtext
Component or Action
===================

Synopsis(Optional)
------------------

If script/command call, show the generalized invocation. Example:

`command [options] [--flags]<input> ...`

If file or environment variables, show where and what to set, accepted value format.
Example:

.. code-block::
    repo/folder/config.sh:
    VAR_NUM = "$VAR_NUM+<numerical value 1–5>"

Description
-----------

What it does/what the purpose is. The results or outcomes. Keep it short and technical.

Describe the **type** of options/flags/values, how they are passed, generated or found.

Variables or options
--------------------
(Change section name as appropriate)

.. confval:: IN_JOKE=<option>
    :default: ``gavel``

    .. option:: gavel

       What the value/option/flag does

    Example Result: ``decided``

    .. option:: helicopter

       Changes state to ultimate goal achieved

       Example Result: ``We made it!``

.. confval:: -h, --help

    Prints help message

Example Usage (optional)
------------------------

Keep it very simple, more showing than explaining.
You can have a sentence or two of what the example achieves.
For example, a fully configured ``local.conf``,
or a CLI tool showing  a common use-case of the tool.
A walk-through/tutorial/how-to belongs in the user-guide.
"A Reference Manual describes the tools from a toolbox,
a User Guide describes how to use one tool from the toolbox."

.. seealso::
   :ref: `related page <ref-page-lable>

   Link to any related user-guide pages, glossary entries, or reference manual pages.
   For inline links like the one above, keep '< >' as they are part of the syntax.
```

### Open Knowledge Format for Internal Documentation

This section serves as a *very* brief overview and introduction.
Read [Google’s blog post](https://cloud.google.com/blog/products/data-analytics/how-the-open-knowledge-format-can-improve-data-sharing) on the format.
The info below summarizes the blog info.

While not currently (August 2026) in use,
The Open Knowledge Format (OKF) is designed to allow sharing of contextual information between individuals, groups, **and** Agents.
While human readable, it aims to be easily consumed by agents.

This information is presented in a wiki like format, designed to be a living library which grows and changes over time.
It is designed to be shared; a new agent or team should have no problem navigating it.
In this way it is much like physical libraries sharing a common organizational system.
While the selection of books differs, discovering what is available remains familiar.

In the format, **knowledge** is represented as a directory of markdown files with YAML front matter containing structured fields.
The directory forms a **bundle**, and each file is a **concept**.
A concept can be any knowledge (data tables, APIs, playbooks).

The front matter has the following fields:

```yaml
---
type:
title:
description:
resource:
tags:
timestamp:
---
```

Concepts are linked using Markdown, where say a table concept links to two datasets to correlate.

## Markup Languages

This section discusses the way that things are laid out **prior** to rendering.

### Why Markup Style Matters

*If it all ends up looking the same in the docs or a blog post, why bother?*

The goal is to make raw content that is:

- simpler for others to review and copyedit or provide GitHub PR review “suggestions”
- clean, structured, and consistent across multiple contributors
- is readable as text files; this is especially important for READMEs.

Another goal is to aid in writing mindfully.
As readers, we have limited bandwidth; extra words and run-on sentences negatively impact throughput.

Guidelines such as column length and semantic line breaks encourage effective writing with short sentences and discrete thoughts.

### General Guidelines

> [!NOTE]
> Inline hyperlinks and text formatting marks are granted an exception to the following rules.
> They can be kept on separate lines to assist with keeping a clean look.

#### Semantic Linebreaks

- **Each new sentence OR thought should be on a separate line.**

Exceptions exist, such as if the sentences are closely related, short, and fit on the same line.

For more information and specification, <https://sembr.org/>

#### Line Column Length

- **Aim to keep lines under 100 characters/line column length.**

There are two ways to address this:

1. Trim the sentence by removing unnecessary words
1. Line break after a punctuation mark, ideally where there is a change in clause.
   Semicolons and colons are good candidates.

Setting column marker in your text editor can assist with this.

#### Table Layout

- **Tables should have row and columns that line up**

Each cell should be the same size.
This helps with parsing it as a plain text file.

## Suggestions and Tips For Writing Documentation

- Say more with less.
  Try deleting every word until doing so would change the meaning.
- Utilize the doc PR template.
  This provides a [checklist](https://github.com/foundriesio/docs/blob/master/.github/pull_request_template.md) which increases the chance for a quick merge.
- Ask for review by people outside of your immediate team.
  Writing a tutorial? Have someone outside of engineering take a look for readability.
  Creating promotional material? Have a engineer check for technical accuracy.
- Always check for ambiguity; is it possible for a segment to have more than one meaning? Be explicit.

### Resources

Linter rules, the Foundries style guide, and Agent skill files can be found in the
[fio-style](https://github.com/foundriesio/fio-style.html) repo.

- Foundries tech writer: [katrina.prosise](mailto:kprosise@quicinc.com)

#### Useful Tools

[Vale](https://vale.sh/) is used for documentation linting.
If you use vim, also install [ALE](https://github.com/dense-analysis/ale),
which integrates useful linting tools  — most which need to be installed separately  —  for checking text in the buffer.
