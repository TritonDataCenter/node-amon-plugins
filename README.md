# amon-plugins

A node.js package for amon-agent plugins shared between amon-master,
amon-relay, amon-agent Triton components.

(This repository is part of the Joyent Triton project. See the [contribution
guidelines](https://github.com/joyent/triton/blob/master/CONTRIBUTING.md) --
*Triton does not use GitHub PRs* -- and general documentation at the main
[Triton project](https://github.com/joyent/triton) page.)


## Usage

For now, use the source.


## Development

The following sections are about developing this module.

### Commiting

Before commit, ensure that the following passes:

    make check

Also see the note at the top that https://cr.joyent.us is used for code review
for this repo.

### Releasing

Changes with possible user impact should:

1. Add a note to the [changelog](./CHANGES.md).
2. Bump the package version appropriately (major for breaking changes, minor
   for new features, patch for bug fixes).
3. Once merged to master, the new version should be tagged (currently this
   does not publish to npm) via:

        make cutarelease

