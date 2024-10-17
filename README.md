<!-- markdownlint-disable MD041 -->
<!-- markdownlint-disable MD033 -->
<!-- markdownlint-disable MD028 -->
<!-- markdownlint-disable MD024 -->

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

[![pre-commit][pre-commit-shield]][pre-commit-url]
[![taskfile][taskfile-shield]][taskfile-url]
[![Terraform][terraform-shield]][terraform-url]
[![Remote State file][statefile-shield]][statefile-url]

# Customer Terraform Infra

Infrastructure as Code (IaC) with Terraform.

## Template introductions - remove me when initialized

- README.md: update h1
- README.md: update link to remote state file below

<details>
  <summary style="font-size:1.2em;">Table of Contents</summary>
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Code-Style](#code-style)
  - [Terraform](#terraform)
- [Getting Started](#getting-started)
  - [Prerequisties](#prerequisties)
  - [Initialize repository](#initialize-repository)
- [Configuration](#configuration)
  - [Preparation](#preparation)
  - [Howto add resources](#howto-add-resources)
- [Known Issues](#known-issues)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
</details>

## Code-Style

### Terraform

#### Best practices

[terraform-best-practices.com][terraform-best-practices]

#### Naming of Terraform resources

- lower-case characters
- underscores

Pattern: `[a-z_]+`

#### Naming of Google Cloud resources

- lower-case characters
- hyphen

Pattern: `[a-z-]+`

## Getting Started

### Prerequisties

- [terraform][terraform-url]
- [pre-commit][pre-commit-url]
- [terraform-docs][terraform-docs]
- [tflint][tflint]
- [yamllint][yamllint]

### Initialize repository

Terraform and pre-commit framework need to get initialized.

```console
task terraform:init
task pre-commit:init
```

## Configuration

### Preparation

All changes require a PR and review. Create a new branch and reference a Jira ticket, f.e.

```console
git switch -c feature/INPRO-1-configure-resource
```

### Howto add resources

#### Terraform

<!-- TBD -->

## Known Issues

<!-- TBD -->

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->

<!-- Links -->

[terraform-best-practices]: https://www.terraform-best-practices.com/naming
[terraform-docs]: https://github.com/terraform-docs/terraform-docs
[tflint]: https://github.com/terraform-linters/tflint
[yamllint]: https://github.com/adrienverge/yamllint

<!-- Badges -->

[pre-commit-shield]: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit
[pre-commit-url]: https://github.com/pre-commit/pre-commit
[taskfile-url]: https://taskfile.dev/
[taskfile-shield]: https://img.shields.io/badge/Taskfile-Enabled-brightgreen?logo=task
[terraform-shield]: https://img.shields.io/badge/terraform-1.x-844fba?logo=terraform
[terraform-url]: https://www.terraform.io/
[statefile-shield]: https://img.shields.io/badge/GCS-tfstate-F8991D.svg?logo=googlecloud
[statefile-url]: https://console.cloud.google.com/storage/browser/customer-tf-states/customer-terraform-infra
