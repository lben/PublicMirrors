# PublicMirrors

Public mirrors of binaries published by their upstream projects. Files are hosted as release assets, with links to their original sources and SHA-256 checksums.

## Graphviz 16.1.0 — EL8 / x86_64

Official Graphviz binaries built for **Rocky Linux 8.9**, part of the Enterprise Linux 8 family. The full archive contains `16.1.0-1.el8.x86_64` packages and architecture-independent (`noarch`) packages.

| Download | Contents |
| --- | --- |
| [Full RPM package archive](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/rocky_8.9_graphviz-16.1.0-rpms.tar.xz) | Official archive containing RPMs, libraries, plugins, and optional packages. |
| [Single RPM built with CMake](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/rocky_8.9_graphviz-16.1.0-cmake.rpm) | Upstream's alternative packaging, with its own dependencies. |
| [SHA256SUMS](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/SHA256SUMS) | Checksums calculated after downloading the official files. |
| [download.sh](https://github.com/lben/PublicMirrors/releases/download/graphviz-16.1.0-el8-x86_64/download.sh) | Downloads and verifies the full archive from this mirror; does not install packages. |

[View the mirror release](https://github.com/lben/PublicMirrors/releases/tag/graphviz-16.1.0-el8-x86_64).

### Verification

Download the binaries you need and `SHA256SUMS` into the same directory. On RHEL 8, verify the downloaded files with:

```sh
sha256sum --check --ignore-missing SHA256SUMS
```

Local checksums and the internal digests of the single RPM and the main RPMs (`graphviz`, `graphviz-libs`, `graphviz-nox`, and `graphviz-plugins-core`) were verified. Execution on RHEL 8 has not been tested; installation depends on the repositories and libraries available on the target system.

### Sources and licenses

- [Official Graphviz 16.1.0 release](https://gitlab.com/graphviz/graphviz/-/releases/16.1.0).
- [Original RPM archive](https://gitlab.com/api/v4/projects/4207231/packages/generic/graphviz-releases/16.1.0/rocky_8.9_graphviz-16.1.0-rpms.tar.xz).
- [Original CMake RPM](https://gitlab.com/api/v4/projects/4207231/packages/generic/graphviz-releases/16.1.0/rocky_8.9_graphviz-16.1.0-cmake.rpm).
- [Official source code for the same version](https://gitlab.com/api/v4/projects/4207231/packages/generic/graphviz-releases/16.1.0/graphviz-16.1.0.tar.xz).

The binaries are redistributed without modification and retain their original licenses. This repository is an independent mirror of the Graphviz project.
