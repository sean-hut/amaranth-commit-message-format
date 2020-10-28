# Amaranth Commit Message Format

## Commit Message Structure

These are the valid commit message structures:

- Summary Line
    1. Summary line

- Summary Line and Body
    1. Summary line
    1. One blank line
    1. Body

- Summary Line and Footer
    1. Summary line
    1. One blank line
    1. Footer

- Summary Line, Body and Footer
    1. Summary line
    1. One blank line
    1. Body
    1. One blank line
    1. Footer

## ASCII

The characters in the commit message must be [ASCII characters][ascii].

[ascii]: <https://en.wikipedia.org/wiki/ASCII#Character_set>

## Summary Line

A commit message must have a summary line.

The summary line is the first line of the commit message.

- The summary is one line.
- The summary line can not be only a [category abbreviation](#category-abbreviation).
- The summary must not be more than 50 characters.
- The summary must not end with a period.
- The summary must start with one of the [category abbreviation](#category-abbreviation) for example **`B`**.
- The summary's first word after the category abbreviation must be lower case.
- The summary must use the imperative mood.  See [imperative mood](#imperative-mood).

## Body

The commit message can have an optional body.

The body explains what changed and the rational for why it changed.

- The body can be multiple lines.
- The body can not contain blank lines.
- The body must use the imperative mood.  See [imperative mood](#imperative-mood).
- The body lines must wrap at 72 characters.
- The body can contain bullet points that start with `-` or `*`.

## Footer

The commit message can have an optional footer.

The footer is for referring to issue IDs.

- The footer can be multiple lines.
- The footer can not contain blank lines.
- Footer lines must start with `Resolves:` or `See also:`
- Footer lines must have one or more issue IDs following each `Resolves:` or `See also:`

Footer line examples:
`Resolves: <issue-id>`
`See also: <issue-id>, <issue-id>`

## Category Abbreviation

These category abbreviation are sorted alphabetically.

- **AA** (API Additions)

    Adding functionality to the API.  For example:

    - Adding user facing features
    - Adding user configurations

- **AR** (API Removals)

    Removing functionality from the API. For example:

    - Removing user facing features
    - Removing user configurations

- **B** (Build)

    Changes that effect the build tools.  For example:

    - Changes to the Makefile.

- **BF** (Bug Fix)

    Fixing an error in the source code.

- **C** (Configuration)

    Changes to configurations.  For example:

    - .gitignore

- **CT** (Contributing)

    Use this when the commit is for managing contributing requirements  For example:

    - Adding a gpg2 elliptic-curve signing key and fingerprint.
    - Signing a contributor agreement.
    - Setting up contributing directories.
    - Revoking a signing key and resigning with a new key.

- **D** (Documentation)

    Changes to documentation.  For example:

    - README.md
    - CHANGELOG.md
    - Texinfo file

- **DD** (Developer Dependencies)

    Changes to developer dependencies.  Developer dependencies are
    programs developers need to have installed.

- **IV** (Increment Version)

    Increment a version number.

- **M** (Merge)

    Merging a branch into another branch.

- **R** (Refactor)

    Changes that do not effect the API and do not add or remove features.

- **RD** (Runtime Dependencies)

    Changes to the projects runtime dependencies.  Runtime dependencies
    are programs the users need to have installed.

- **RV** (Revert)

    Reverting a commit.

- **T** (Test)

    Adding or changing tests.

## Imperative Mood

- Add not Added nor Adds
- Remove not Removed nor Removes
- Fix not Fixed nor Fixes
