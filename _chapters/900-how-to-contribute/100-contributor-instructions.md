---
title: Contributor Instructions
slug: contributor-instructions
---
## Get Involved

_Placeholder: we need to write a general call for community contributions
here at some point. This should include instructions for how to edit
on github, creating a pull request for review._


## Markdown

When editing page contents, we generally prefer to use **Markdown format**.
This is a plain text markup notation that is quick to learn and easy
to edit. For details, read:

+ [GitHub's "Getting Started" page on: Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
+ [GitHub's docs on writing Markdown for GitHub use](https://docs.github.com/en/get-started/writing-on-github)
+ [Markdown cheat sheet](https://github.com/adam-p/markdown-here/wiki/markdown-cheatsheet)

Note that HTML content can be embedded in markdown files as well. And if you
want to write vanilla HTML content for a new play instead of using markdown,
you can convert the play template to HTML, keep the metadata section at the
start, but write all the content using HTML markup and give the file a
`.html` extension instead of `.md`.


## Discuss a Play

_Placeholder: we want to write a short description about sharing
experiences or knowledge about specific plays in the play's corresponding
discussion section, with a reference
to {% include chapter-link.html slug="join-discussions" %}._


## Contributing New Plays

_Placeholder: we need to briefly discuss the licensing for contributions to
this book, and probably include a link to the LICENSE file._

Here is the process for contributing a new play to this book:

1. Decide on a **name** for the play. Choose a clear, evocative name
   (preferably a noun phrase) that future educators can use as a recognizable
   way to identify or talk about this play.
2. Make a copy of the {% include chapter-link.html slug="play-template" %}
   file in this repository, which is located
   at `_chapters/900-how-to-contribute/200-play-template.md`.
3. Fill in the content! Place your play's **name** in the "title:" field
   at the top of the file in the metadata section. Also, add a "slug", or
   the human-readable URL-style page name for this play. This must be unique,
   since it will be used as a unique way to link to the play. We recommend just
   lower-casing the name, with spaces replaced by dashes and special characters
   removed. Then see the explanations below for what you should
   put in each section in the template.
4. Add your your file to this
   project's {% include chapter-link.html slug="incubator" %} by placing it in
   the `_chapters/800-incubator` directory. The file name should follow the
   basic format of `ddd-slug.md`, where `ddd` is a number, `slug` is the
   slug you've entered in the page's metadata, and `.md` is the file extension.
   Just look at the existing files already in that directory, find the highest
   number, and add 10 so your new play will go at the end numerically. If
   there are no other plays currently in the incubator, number yours 010.
5. Plays added in the {% include chapter-link.html slug="incubator" %} will
   be reviewed and moved to an appropriate chapter.
6. Check it in and create a pull request to send your contribution to github
   for review!

## Play Sections

Each play is written in a style similar
to [software design patterns](https://www.martinfowler.com/articles/writingPatterns.html).
They have a common set of sections that are intended to prompt play writers
to consider the key aspects that others need in order to consider adopting
a play, and also intended to help other educators know where to look for
key information in the play's description. The following explanations
describe the sections that appear in each play:

+ **Name**: The play's name is intended to be a short, evocative label
  that the community can use to refer to the play. We prefer titles that
  are noun phrases that aren't too long, nor too generic.
+ **Intent**:  A slightly longer one-sentence (or at least
  concise) description of what the play achieves--that is, what is the
  purpose or intent of using the play?
+ **Problem**: A concise description of the problem or situation that
  the play solves or addresses, answering the question of: why use it?
+ **Solution**: The main description of the play and all of its elements
  or components, in enough detail so the reader can understand how it works.
+ **Applicability**: Describes the context(s) where this play works, and
  the tradeoffs that should be considered in deciding whether or not to
  use it.
+ **How to Implement**: Provides any implementation details or techniques
  about how to actually deploy the play--how do you "make it work". This
  section should provide enough detail so that another educator would know
  how to implement the  play in their own classroom.
+ **See Also**: A bullet list of related plays.
+ **Source**: A citation to the publication, web page, or source of the
  play, plus the name of the person who wrote up its description.
+ **References**: Any other references that describe more about the play.
+ **Community Discussion**: A "public comments" section where community
  members can share their own experiences, observations, questions, or
  perspectives on the play.

## Advanced Features

This book is written using [jekyll](https://jekyllrb.com/) and
the [jekyll-chapterbook](https://github.com/jasongrimes/jekyll-chapterbook) theme.
See the [jeykll-chapterbook README](https://github.com/jasongrimes/jekyll-chapterbook?tab=readme-ov-file) for details on some of the theme's
more advanced features if you want to do something beyond basic markdown,
such as including figures, linking to other plays, linking to references
in the reference section, etc.
