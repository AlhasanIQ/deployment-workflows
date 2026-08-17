# deployment-workflows

Small reusable GitHub Actions workflows for AlhasanIQ services:

- `go-build.yml` — checkout, pinned Go setup, test/vet/build, artifact upload;
- `bun-build.yml` — checkout, pinned Bun setup, install/test/lint/build, upload;
- `publish-artifact.yml` — package and publish an arbitrary repository artifact.

Callers pin these workflows by full commit SHA. Builds use GitHub-hosted runners,
so application repositories do not need access to the private deployment runner
or home tailnet.
Reusable CI workflows for AlhasanIQ services
