# Contributing to Artefacts

We'd love to accept your contributions to make this project even better than it is today!

As a contributor, here are the guidelines we would like you to follow:

- [Getting started](#Getting-started)
- [Commit Messages Guidelines](#Commit-Messages-Guidelines)
- [Documentation Guidelines](#Documentation-Guidelines)
- [Dependencies Guidelines](#Dependencies-Guidelines)
- [Dev mode vs Prod mode](#Dev-mode-versus-production-mode)

## Getting started

If you already have `git` and `VS Code` installed on your machine:

  Clone this repository:
  
  ```bash
  git clone https://github.com/Zoroastrian-Digital-Humanities/Artefacts.git
  cd Artefacts
  ```

Otherwise, open the repository with GitHub Desktop.

## Working with VS Code

If you are using VS Code, it is recommanded to install the recommanded extensions.

## Working with GitHub Desktop

TBD

## Guidelines to add a new Artefact

Basically an artefact is a folder within the `src` folder, which contains a `readme.md` file (a Markdown file), one or more image files, zero or one `map.geojson` file (geo data file).

## Markdown Guidelines

- You should follow this [GitHub Guide on Markdown](https://guides.github.com/features/mastering-markdown/)

## Commit Messages Guidelines

Commit messages should follow the Semantic Commit Messages format:

```txt
label(namespace): title
```

`label` is one of the following:

- `chore` - build-related work, a change in the package.json file, a change in a configuration  file or a change to a script file.
- `docs` - changes to a markdown file
- `feat` - a new feature.
- `fix` - a fix, either in code or in an artefact.
- `refactor` - a code change that neither fixes a bug nor adds a feature
- `style` - a change in the code style: spaces/alignment/wrapping etc.
- `test` - adding missing tests or correcting existing tests.

`namespace` is put in parentheses after label and is mandatory. Must be lowercase.

`title` is a brief summary of changes.

Examples:

```txt
feat(artefact): add first page of Khordeh Avesta
docs(artefacts): update curated artefacts list
fix(artefact): fix typo in first page of Khordeh Avesta
...
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
