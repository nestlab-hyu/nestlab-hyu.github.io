# AGENTS.md

## Project overview

This repository contains the source code for the lab homepage.

Treat this project as a public-facing academic lab website. Prioritize correctness, clarity, maintainability, and minimal changes. Do not make broad redesigns unless explicitly requested.

## General workflow

Before modifying files:

1. Inspect the repository structure.
2. Identify the framework or static site generator used by the project.
3. Identify where pages, components, styles, assets, and data files are located.
4. Explain the intended change plan briefly.
5. Do not modify files until the requested target is clear.

When modifying files:

1. Keep the existing design style and layout unless the user explicitly asks for redesign.
2. Make the smallest reasonable change.
3. Avoid unrelated refactoring.
4. Do not remove existing content unless explicitly requested.
5. Preserve existing naming conventions, formatting, and directory structure.
6. Avoid adding new dependencies unless absolutely necessary.
7. Do not modify deployment configuration unless the task requires it.

After modifying files:

1. Summarize the changed files.
2. Explain the purpose of each change.
3. Show how to test the website locally.
4. Run the relevant build, lint, or test command when available.
5. Report any command failure honestly, including the command and error summary.

## Git safety rules

Do not commit automatically unless explicitly asked.

Do not push to remote branches unless explicitly asked.

Prefer working on a separate branch rather than directly on `master`.

Recommended branch name format:

```bash
update-homepage-<short-topic>
```

Before making changes, check:

```bash
git status
```

After making changes, check:

```bash
git diff
git status
```

## Website content rules

This is an academic lab homepage. Keep writing concise, professional, and appropriate for a computer science research lab.

Avoid exaggerated marketing language.

Prefer clear academic wording such as:

* research
* systems and network security
* Internet infrastructure security
* PKI/TLS/DNS security
* AI agent security
* trusted execution environments
* program analysis
* fuzzing
* privacy-preserving systems

Use “lab” consistently unless the existing website uses another term.

Use “homepage” or “website” consistently based on the existing wording.

## Editing scope

For homepage updates, first locate the main homepage file and any shared data/config files.

For people/member updates, first locate whether member information is stored in:

* a Markdown file
* a YAML/JSON data file
* a JavaScript/TypeScript object
* a template/component file

For publication updates, first locate whether publications are stored in:

* BibTeX
* Markdown
* YAML/JSON
* HTML
* JavaScript/TypeScript

Do not guess the data format. Inspect the existing implementation first.

## Style rules

Preserve the existing visual style.

Do not introduce heavy animations.

Do not introduce a new CSS framework.

Do not rewrite all CSS unless explicitly requested.

Prefer simple black-and-white or existing theme colors.

Make pages readable on desktop and mobile when the existing project supports responsive layout.

## Build and test

After changes, identify the correct local commands from the repository.

Common examples include:

```bash
npm install
npm run build
npm run dev
```

or:

```bash
bundle install
bundle exec jekyll serve
```

Do not assume these commands are correct without checking package files or project documentation.

## Communication style

When responding to the user:

1. Be concise.
2. Explain what was changed and why.
3. Mention files by path.
4. Mention commands that were run.
5. Clearly say when something was not tested.
6. Ask for clarification only when the requested change is ambiguous enough that proceeding may cause incorrect edits.

## Important constraints

Do not modify unrelated files.

Do not reformat the entire repository.

Do not change generated files unless necessary.

Do not expose secrets, tokens, credentials, or private information.

Do not add placeholder content that looks final unless the user requested placeholders.

Do not invent lab members, publications, projects, or affiliations.

