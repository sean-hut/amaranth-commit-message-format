# Amaranth Commit Message Format

## Commit Message Structure

These are the valid commit message structures:

- Summary Line and Sign Off Line
    1. Summary line
    2. One blank line
    3. Sign off line
    4. One blank line

- Summary Line, Body and Sign Off Line
    1. Summary line
    2. One blank line
    3. Body
    4. One blank line
    5. Sign off line
    6. One blank line

- Summary Line, Footer and Sign Off Line
    1. Summary line
    2. One blank line
    3. Footer
    4. One blank line
    5. Sign off line
    6. One blank line

- Summary Line, Body, Footer and Sign Off Line
    1. Summary line
    2. One blank line
    3. Body
    4. One blank line
    5. Footer
    6. One blank line
    7. Sign off line
    8. One blank line

## ASCII

The characters in the commit message must be [ASCII characters][ascii].

[ascii]: <https://en.wikipedia.org/wiki/ASCII#Character_set>

## Summary Line

A commit message must have a summary line.

The summary line summarizes the commit.

- The summary line is the first line of the commit message.
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
- The body must not contain footer lines.

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

## Sign Off Line

The commit message must have a sign off line.

The sign off line is created by `git` when you use `git commit`'s
`--signoff` option.

Here is an example of a sign off line:

`Signed-off-by: <NAME> <EMAIL>`

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

- **FA** (Functionality Addition)

    Add functionality that does not change the API.

- **FR** (Functionality Removal)

    Remove functionality that does not change the API.

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
