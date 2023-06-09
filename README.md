# Workshop: Git, GitHub, Markdown

[Link to presentation](https://alicemcgrath.digital.brynmawr.edu/pres/git-hub.html)

[Something](something.md)

[Installation instructions](#installation-instructions)

[Versioning vocabulary](#versioning-vocabulary)

[Markdown syntax](#markdown-syntax)

[GitHub Pages & Jekyll](#github-pages-instructions)

## Installation instructions

Before we get started, please:

1. Sign up for a GitHub account at [github.com](https://github.com/)
2. Install Visual Studio Code: [code.visualstudio.com](https://code.visualstudio.com/)
3. Install Git, following these instructions: [git-scm.com/download](https://git-scm.com/download) 

## Versioning Vocabulary

**Repo or repository** (n.) 
: A discrete project on GitHub that contains a set of files, a change history, and a set of contributors. (E.g. [this one](https://github.com/digbmc/dssf-syll))

**Fork** (v.)
: To copy a repo's files and version history to a new one with its own settings (preserves connection with original repo but doesn't interfere). 

**Clone** (v.)
: To download a local copy of a repo on GitHub with a tracked connection to the remote repo.

**Local** (adj.)
: On your computer.

**Remote** (adj.)
: On someone else's computer (aka 'the cloud').

**Branch** (n.)
: A version of a repository with its own history. Branches can be created for a unique set of changes and later *merged* with the main branch to avoid file conflicts.

**Commit** (n.)
: A discrete set of changes to a project that have been packaged and labeled.

## Markdown Syntax

```{md}

# First level heading 

## Second-level heading

Paragraph with **bold** text and *italicized* text. 

[This is linked text](www.myurl.com)

![This is an image with alt text](imageurl.jpg)

```

See also this [cheat sheet](https://www.markdownguide.org/cheat-sheet/) for more markdown syntax.

## GitHub Pages instructions

- Open your github pages site project workspace in VS Code and open a terminal (or GitBash) window

- Make sure you have Jekyll installed properly:
```
jekyll --version
```
- Download [this Gemfile](https://github.com/digbmc/git-hub-ws/blob/gh-pages/Gemfile) and add it to the root folder of your repository

- Install the necessary dependencies for this site by running:
```
bundle install
```
- Now you're ready to create a 'test serve' of your site:
```
bundle exec jekyll serve
```
- If this works, you should see the message:
```
    Server address: http://127.0.0.1:400
  Server running... press ctrl-c to stop.
```
- Copy and paste the server url into a browser to see a preview of your site!
- As you edit your site, this preview will update
- If you make changes to your `_config.yml` file, you'll need to stop the server (`ctrl-c`) and run it again: `bundle exec jekyll serve`
- When you're done working, be sure to stop your server before you close your laptop
