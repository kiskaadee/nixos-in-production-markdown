# NixOS in Production, by Gabriella Gonzalez (Markdown Edition)

An ordered, cleanly formatted Markdown edition of Gabriella Gonzalez's book, [*NixOS in Production*](https://github.com/Gabriella439/nixos-in-production).

---

> [!IMPORTANT]
> ### 📖 Support the Author — Get the Book on Leanpub!
> Gabriella Gonzalez published *NixOS in Production* under an open license because she believes digital scarcity shouldn't lock away technical knowledge. She self-published and paid out-of-pocket for all professional editing and layout services. Along the way, she also contributed foundational improvements to the Nix ecosystem—including [Terraform support for NixOS](https://www.haskellforall.com/2023/01/terraform-nixos-ng-modern-terraform.html) and [Linux builders on macOS](https://www.haskellforall.com/2022/12/nixpkgs-support-for-linux-builders.html).
>
> If this guide helps you or your organization, please consider purchasing the official edition on Leanpub:
>
> 👉 **[Purchase the Leanpub Edition of *NixOS in Production*](https://leanpub.com/nixos-in-production)**
>
> Purchasing the Leanpub edition directly supports independent technical writing and entitles you to a discount on the forthcoming print edition!

---

## About This Project

Gabriella Gonzalez's ***NixOS in Production*** is an invaluable practical guide for introducing, configuring, and operating NixOS in enterprise and production environments.

The original book manuscript is tailored for Leanpub publication, where chapter sequence is declared through metadata files rather than filesystem naming. 

When browsing on GitHub, unnumbered files sort alphabetically rather than narratively.

This repository provides an **ordered, reader-friendly Markdown edition** designed for:

- Sequential reading directly in the GitHub web interface.
- Easy reading through local Markdown viewers, offline readers, and editors.
- Clean formatting and cross-chapter navigation.
- Original content is preserved as-is.

---

## Table of Contents

The chapters below are organized in their intended reading order:

1. [01. Introduction](chapters/01-introduction.md) — Scope, target audience, and philosophy.
2. [02. Motivation](chapters/02-motivation.md) — Why NixOS in production: reproducibility, declarative configuration, and eliminating state drift.
3. [03. The Big Picture](chapters/03-big-picture.md) — High-level architecture and how NixOS machines are built and deployed.
4. [04. Setup](chapters/04-setup.md) — Preparing your workstation and Nix environment.
5. [05. Web Server](chapters/05-web-server.md) — Building and provisioning your first declarative service.
6. [06. Modules](chapters/06-modules.md) — The anatomy of NixOS modules: `options`, `config`, and abstraction.
7. [07. Advanced Modules](chapters/07-advanced-modules.md) — Submodules, types, assertions, and composing complex services.
8. [08. Terraform](chapters/08-terraform.md) — Integrating NixOS deployments with infrastructure-as-code.
9. [09. Continuous Integration & Deployment](chapters/09-continuous-integration-deployment.md) — Automated builds, caches, and rollout pipelines.
10. [10. Flakes](chapters/10-flakes.md) — Hermetic inputs, flake locks, and standardized outputs.
11. [11. Integration Testing](chapters/11-integration-testing.md) — Running declarative multi-node NixOS VM tests.
12. [12. Containers](chapters/12-containers.md) — Packaging and orchestrating OCI/Docker containers with Nix.

---

## Upstream Templates & Code

The code templates, Nix expressions, and sample projects referenced throughout the book are maintained in the upstream repository's [`templates/`](https://github.com/Gabriella439/nixos-in-production/tree/main/templates) directory and can be initialized with `nix flake init`:

```bash
# Example: initialize the server template from upstream
nix flake init --template github:Gabriella439/nixos-in-production#server
```

---

## Attribution & License

- **Original Author:** Gabriella Gonzalez ([@Gabriella439](https://github.com/Gabriella439))
- **Original Repository:** [Gabriella439/nixos-in-production](https://github.com/Gabriella439/nixos-in-production)
- **Official Edition:** [Leanpub](https://leanpub.com/nixos-in-production)

Both the original work and this adapted edition are licensed under the **[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License (CC BY-NC-SA 4.0)](LICENSE)**.
