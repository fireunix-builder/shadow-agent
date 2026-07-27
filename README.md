# Shadow Agent Builder

Public build and release automation for the private
`fireunix-app/shadow-agent` repository.

The private source is checked out only on an ephemeral GitHub-hosted runner
using a repository-scoped, read-only PAT. This repository and its caches never
contain private source or project build output. Release archives contain only
compiled binaries and explicitly published runtime templates.

Run the `Release` workflow manually with a source ref and version. Published
artifacts are attached to this repository's GitHub Release.

