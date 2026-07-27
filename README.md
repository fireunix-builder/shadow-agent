# Shadow Agent Builder

Public build and release automation for the private
`fireunix-app/shadow-agent` repository.

The private source is checked out only on an ephemeral GitHub-hosted runner
using a repository-scoped, read-only PAT. This repository and its caches never
contain private source or project build output. Release archives contain only
compiled binaries and explicitly published runtime templates.

Run the `Release` workflow manually with a source ref and version. GitHub
Releases are written back to the private source repository through a separate
single-repository write token. This public repository never hosts Releases;
R2 receives only the reviewed binary archives and checksums.
The requested release tag must already exist in the private source repository.
