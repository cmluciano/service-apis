# Release Process

## Overview

The Service APIs project is an API project that has the following two components:
- Kubernetes Custom Resource Definitions (CRDs)
- Corresponding Go API in the form of `sigs.k8s.io/service-apis` Go package

This repository is the home for both of the above components.

## Versioning strategy
The versioning strategy for this project is covered in detail in [the release
documentation].

[the release documentation]: https://kubernetes-sigs.github.io/service-apis/releases/#versioning

## Releasing a new version

- Write the [changelog](CHANGELOG.md) with user-visible API changes. This must
  go through the regular PR review process and get merged into the `master` branch.
  Approval of the PR indicates community consensus for a new release.
- Once the above PR is merged, the author must publish a new Git tag. This can
  be done using the `git` CLI or Github's [release][release]
  page. This step can be performed only by [Service APIs maintainers][service-apis-team].

[release]: https://github.com/kubernetes-sigs/service-apis/releases
[service-apis-team]: https://github.com/kubernetes/org/blob/master/config/kubernetes-sigs/sig-network/teams.yaml

