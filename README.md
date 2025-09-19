# containerd

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&logoColor=white)](https://github.com/rolehippie/containerd)
[![General Workflow](https://github.com/rolehippie/containerd/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/containerd/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/containerd/actions/workflows/docs.yml/badge.svg)](https://github.com/rolehippie/containerd/actions/workflows/docs.yml)
[![Galaxy Workflow](https://github.com/rolehippie/containerd/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/containerd/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/containerd)](https://github.com/rolehippie/containerd/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.containerd-blue)](https://galaxy.ansible.com/rolehippie/containerd)

Ansible role to install and configure containerd.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [containerd_fixed_version](#containerd_fixed_version)
  - [containerd_keyring](#containerd_keyring)
  - [containerd_skip_config](#containerd_skip_config)
  - [containerd_skip_service](#containerd_skip_service)
  - [containerd_upstream_arch](#containerd_upstream_arch)
  - [containerd_upstream_version](#containerd_upstream_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`

## Default Variables

### containerd_fixed_version

Install and pin a specific version

#### Default value

```YAML
containerd_fixed_version:
```

### containerd_keyring

Path for the repository keyring

#### Default value

```YAML
containerd_keyring: /usr/share/keyrings/containerd-archive-keyring.gpg
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
containerd_upstream_arch: "{{ 'arm64' if ansible_architecture == 'aarch64' or ansible_architecture
  == 'arm64' else 'amd64' }}"
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
