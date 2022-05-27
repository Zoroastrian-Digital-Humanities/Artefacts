# Contributing to Artefacts

We'd love to accept your contributions to make this project even better than it is today!

As a contributor, here are the guidelines we would like you to follow:

- [Getting started](#Getting-started)
- [Commit Messages Guidelines](#Commit-Messages-Guidelines)
- [Markdown Guidelines](#Markdown-Guidelines)
- [Dependencies Guidelines](#Dependencies-Guidelines)

## Getting started

If you already have `git` and `VS Code` installed on your machine:

  Clone this repository:
  
  ```bash
  git clone https://github.com/Zoroastrian-Digital-Humanities/Artefacts.git
  cd Artefacts
  ```

## Working with git

To install `Git` on your machine, follow the instructions on [GitHub](https://github.com/git-guides/install-git).

For a complete installation guide, follow the instructions [here](https://git-scm.com/book/en/v2).

## Working with VS Code

To install VS Code, follow the instructions on [this page](https://code.visualstudio.com).

When using VS Code, it is recommanded to install the recommanded extensions.

## Guidelines to add a new Artefact

Basically an artefact is a folder within the `src` folder, which contains a `readme.md` file (a Markdown file), one or more image files, zero or one `map.geojson` file (geo data file).

The `readme.md` file is the main documentation of the artefact. It should always start with a metadata section, which is a list of key-value pairs separated by a colon and a space:

```markdown
---
type: 
location:
found-at: 
period: 
dimensions: 
presented-by: 
museum: 
copyright:
source: 
photograph: 
tags: 
---
```

Then it should contain a title, a description.

If you need to insert images inside that markdown file, you should upload one or more images in the same folder and the image file names should follow the `kebab` file naming convention (more info [here](https://github.com/ayushi7rawat/Youtube-Projects/tree/master/Case%20style%20in%20programming?ref=morioh.com&utm_source=morioh.com#case-style-in-programming)):

- all characters in the file name are in lower case
- no special characters like `?`, `%`, etc ...
- spaces between words should be replaced by the `-` character

Examples of correct image file names:

- `anquetil-duperron.png`

Examples of incorrect file names:

- `Anquetil Duperron.png`

## Markdown Guidelines

- You should follow this [GitHub Guide on Markdown](https://guides.github.com/features/mastering-markdown/)

## Commit Messages Guidelines

Commit messages should follow the Semantic Commit Messages format:

```txt
label(namespace): title
```

`label` is one of the following:

- `chore` - build-related work, a change in the package.json file, a change in a configuration  file or a change to a script file;
- `docs` - changes to a documentation file;
- `feat` - a new feature, a new artefact or an enhancement of an existing artefact;
- `fix` - a fix, either in code or in an artefact;
- `refactor` - a code change that neither fixes a bug nor adds a feature;
- `style` - a change in the code style: spaces/alignment/wrapping etc.;
- `test` - adding missing tests or correcting existing tests;

`namespace` is put in parentheses after label and is mandatory. Must be lowercase.

`title` is a brief summary of changes.

Examples:

```txt
feat(artefact): add first page of Khordeh Avesta
docs(artefacts): update curated list of artefacts
fix(artefact): fix typo in first page of Khordeh Avesta
```

If you are not sure about how to lable the commit, or how many files to put in the same commit, you can look at the [commits history](https://github.com/Zoroastrian-Digital-Humanities/Artefacts/commits/main).

### Code Comment

- Comments inside code should be generally avoided. If the code would not be understood without comments, consider re-writing the code to make it self-explanatory.

## Dependencies Guidelines

For all dependencies (both production and development):

- **Do not add** a dependency if the desired functionality is easily implementable.
- If adding a dependency, it should be well-maintained and trustworthy.

A barrier for introducing new production dependencies is especially high:

- **Do not add** production dependency unless it's critical to project success.
