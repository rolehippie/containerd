# containerd

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/containerd) [![Testing Build](https://github.com/rolehippie/containerd/workflows/testing/badge.svg)](https://github.com/rolehippie/containerd/actions?query=workflow%3Atesting) [![Readme Build](https://github.com/rolehippie/containerd/workflows/readme/badge.svg)](https://github.com/rolehippie/containerd/actions?query=workflow%3Areadme) [![Galaxy Build](https://github.com/rolehippie/containerd/workflows/galaxy/badge.svg)](https://github.com/rolehippie/containerd/actions?query=workflow%3Agalaxy) [![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/containerd)](https://github.com/rolehippie/containerd/blob/master/LICENSE)

Ansible role to install and configure containerd.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Default Variables](#default-variables)
  - [containerd_fixed_version](#containerd_fixed_version)
  - [containerd_skip_config](#containerd_skip_config)
  - [containerd_skip_service](#containerd_skip_service)
  - [containerd_upstream_arch](#containerd_upstream_arch)
  - [containerd_upstream_version](#containerd_upstream_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Default Variables

### containerd_fixed_version

Install and pin a specific version

#### Default value

```YAML
containerd_fixed_version:
```

### containerd_skip_config

Skip config if handled by something else

#### Default value

```YAML
containerd_skip_config: false
```

### containerd_skip_service

Skip service if handled by something else

#### Default value

```YAML
containerd_skip_service: false
```

### containerd_upstream_arch

System arch used by upstream repository

#### Default value

```YAML
containerd_upstream_arch: amd64
```

### containerd_upstream_version

Install from upstream repository

#### Default value

```YAML
containerd_upstream_version: true
```

## Discovered Tags

**_containerd_**


## Dependencies

- None

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
