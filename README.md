# nix-playground

A personal hands-on learning lab for the entire Nix ecosystem — the language, the package manager,
flakes, NixOS, Home Manager, nix-darwin, declarative deployments, and beyond.
**197 topics across 20 categories**, designed as a 6–12 month progressive learning path.
The folder numbering IS the learning map: higher number = deeper level.

---

## What is Nix? (quick clarification)

| Thing              | What it is                                                                 |
|--------------------|----------------------------------------------------------------------------|
| Nix (language)     | A pure, lazy, functional language used to describe packages and configs    |
| Nix (pkg manager)  | A package manager that works on Linux and macOS without changing your OS   |
| NixOS              | A full Linux OS built entirely on the Nix package manager                  |
| Flakes             | The modern module system with versioned inputs/outputs (de facto in 2026)  |
| nixpkgs            | The world's largest package repo (80k+ packages)                           |
| Home Manager       | Manages your user environment (dotfiles, apps, shell) declaratively        |
| nix-darwin         | Like NixOS but for macOS system-level config                               |

---

## Legend

**Level:** 🟢 Beginner | 🟡 Intermediate | 🔴 Advanced | 🔵 Expert

**Domain:** 📦 Package manager | 🗣️ Language | 🖥️ NixOS | 🏠 Home Manager | 🍎 macOS | 🚀 DevOps/Infra

---

## Recommended learning path

```
Weeks 1-2:   01 → 02                    (what is Nix + installation)
Weeks 3-5:   03 → 04                    (Nix language + package manager)
Weeks 6-8:   06 → 07                    (flakes + dev shells ← the killer feature)
Weeks 9-11:  05 → 08                    (derivations + deep nixpkgs)
Weeks 12-14: 09 → 10                    (NixOS + Home Manager)
Weeks 15-16: 11 → 18                    (nix-darwin if on Mac + ecosystem tooling)
Weeks 17-20: 12 → 13 → 14              (module system + packaging + CI/CD)
Weeks 21-24: 15 → 16 → 17 → 19        (deployment + cloud + secrets + architecture)
Ongoing:     20                          (ecosystem news and new tools)
```

---

## Category index

| Category | Level / Domain | Summary |
|---|---|---|
| [01 — What is Nix?](./01-what-is-nix/README.md) | 🟢 🗣️📦 | Understand what the Nix ecosystem actually is — language, package manager, and OS — the core problems it solves, and how it compares to alternatives like Docker, Ansible, and Homebrew. |
| [02 — Installation and Setup](./02-installation-and-setup/README.md) | 🟢 📦 | Install and configure Nix on Linux, macOS, and NixOS. |
| [03 — Nix Language](./03-nix-language/README.md) | 🟢🟡 🗣️ | Master the Nix expression language — a pure, lazy, functional language that underpins every package definition and configuration in the ecosystem. |
| [04 — Nix Package Manager](./04-nix-package-manager/README.md) | 🟢🟡 📦 | Learn to use Nix as a day-to-day package manager: installing and removing packages, managing profiles, using ephemeral shells, garbage collecting the store, and working with binary caches. |
| [05 — Derivations](./05-derivations/README.md) | 🟡🔴 📦 | Dive into derivations — the fundamental build units of Nix. |
| [06 — Flakes](./06-flakes/README.md) | 🟡🔴 📦 | Master Nix flakes — the modern, reproducible way to define packages, NixOS configs, dev shells, and more. |
| [07 — Dev Shells and Environments](./07-dev-shells-and-environments/README.md) | 🟡 🚀 | Leverage Nix for per-project, reproducible development environments. |
| [08 — nixpkgs](./08-nixpkgs/README.md) | 🟡🔴 📦 | Explore nixpkgs — the world's largest package repository with 80k+ packages. |
| [09 — NixOS](./09-nixos/README.md) | 🟡🔴 🖥️ | Configure and manage NixOS — the fully declarative Linux distribution. |
| [10 — Home Manager](./10-home-manager/README.md) | 🟡🔴 🏠 | Manage your user environment declaratively with Home Manager — dotfiles, shell config, applications, and development tools, all version-controlled and reproducible. |
| [11 — nix-darwin](./11-nix-darwin/README.md) | 🟡🔴 🍎 | Bring NixOS-style declarative configuration to macOS with nix-darwin. |
| [12 — NixOS Module System](./12-nixos-module-system/README.md) | 🔴🔵 🖥️ | Deep-dive into the NixOS module system — the extensible configuration framework powering NixOS and Home Manager. |
| [13 — Packaging Software](./13-packaging-software/README.md) | 🔴 📦 | Package software of any language — C/C++, Python, Node. |
| [14 — CI/CD and Builds](./14-ci-cd-and-builds/README.md) | 🔴 🚀 | Integrate Nix into your CI/CD pipelines. |
| [15 — Multi-Machine Deployment](./15-multi-machine-deployment/README.md) | 🔴🔵 🚀 | Deploy NixOS configurations to fleets of machines. |
| [16 — Nix in Containers and Cloud](./16-nix-in-containers-and-cloud/README.md) | 🔴🔵 🚀 | Build minimal OCI/Docker images with Nix and run NixOS on every major cloud provider. |
| [17 — Secrets Management](./17-secrets-management/README.md) | 🔴 🚀 | Handle secrets safely in a declarative Nix setup. |
| [18 — Ecosystem Tooling](./18-ecosystem-tooling/README.md) | 🟡🔴 📦 | Survey the rich Nix ecosystem tooling: output monitors, package locators, formatters, linters, diff viewers, documentation tools, and disk analyzers that make working with Nix more productive. |
| [19 — Patterns and Architecture](./19-patterns-and-architecture/README.md) | 🔴🔵 🚀 | Design and structure large-scale Nix repositories. |
| [20 — Emerging and New](./20-emerging-and-new/README.md) | 🔵 📦 | Track the cutting edge of the Nix ecosystem — new implementations, language evolution, commercial platforms, and experimental tools. |

---

## Comparison table

| Topic | Category | Level | Domain | Key command / file | Official docs link | Status |
|-------|----------|-------|--------|-------------------|-------------------|--------|

---

## Progress

### 01 - What is Nix? 🟢
- [ ] 🟢🗣️ Nix: Language vs Package Manager vs OS
- [ ] 🟢📦 Problems Nix Solves
- [ ] 🟢📦 The Nix Store
- [ ] 🟢📦 Derivations the Core Concept
- [ ] 🟢📦 Reproducibility and Purity
- [ ] 🟢📦 Nix vs Docker vs Ansible vs Homebrew
- [ ] 🟢📦 Channels vs Flakes

### 02 - Installation and Setup 🟢
- [ ] 🟢📦 Install Nix on Linux
- [ ] 🟢🍎 Install Nix on macOS
- [ ] 🟢🖥️ Install NixOS
- [ ] 🟢📦 Determinate Systems Installer
- [ ] 🟢📦 Enable Flakes and Nix Command
- [ ] 🟢📦 Basic Nix Config
- [ ] 🟢📦 Nix Shell First Contact

### 03 - Nix Language 🟢🟡
- [ ] 🟢🗣️ Basic Data Types
- [ ] 🟢🗣️ Strings and String Interpolation
- [ ] 🟢🗣️ Lists and Attrsets
- [ ] 🟢🗣️ Functions and Lambdas
- [ ] 🟢🗣️ Let in and Inherit
- [ ] 🟢🗣️ With and Rec
- [ ] 🟢🗣️ If Then Else
- [ ] 🟢🗣️ Import and Builtins
- [ ] 🟡🗣️ Lazy Evaluation
- [ ] 🟡🗣️ Path Types
- [ ] 🟡🗣️ Lib and Useful Functions
- [ ] 🟡🗣️ Practical Exercises

### 04 - Nix Package Manager 🟢🟡
- [ ] 🟢📦 Nix Env Basic Commands
- [ ] 🟢📦 Nix Profile Modern
- [ ] 🟢📦 Searching Packages
- [ ] 🟢📦 Nix Shell Temporary Environments
- [ ] 🟢📦 Nix Run Without Installing
- [ ] 🟡📦 Garbage Collection
- [ ] 🟡📦 Nix Store Query
- [ ] 🟡📦 Rollbacks and Generations
- [ ] 🟡📦 Binary Caches Substituters
- [ ] 🟡📦 Cachix

### 05 - Derivations 🟡🔴
- [ ] 🟡📦 What Is a Derivation
- [ ] 🟡📦 mkDerivation Basics
- [ ] 🟡📦 Build Phases
- [ ] 🟡📦 Dependencies: buildInputs and nativeBuildInputs
- [ ] 🟡📦 Fixed Output Derivations
- [ ] 🟡📦 fetchFromGitHub and Fetchers
- [ ] 🔴📦 patchPhase and Hooks
- [ ] 🔴📦 overrideAttrs
- [ ] 🔴📦 Debugging Failed Builds
- [ ] 🔴📦 Cross Compilation

### 06 - Flakes 🟡🔴
- [ ] 🟡📦 What Are Flakes
- [ ] 🟡📦 Flake Nix Structure
- [ ] 🟡📦 Inputs and Outputs
- [ ] 🟡📦 Flake Lock
- [ ] 🟡📦 Nix Flake Commands
- [ ] 🟡📦 Flake Outputs: packages
- [ ] 🟡📦 Flake Outputs: devShells
- [ ] 🟡📦 Flake Outputs: apps
- [ ] 🟡🖥️ Flake Outputs: nixosConfigurations
- [ ] 🟡🏠 Flake Outputs: homeConfigurations
- [ ] 🔴📦 Flake Outputs: overlays and modules
- [ ] 🔴📦 follows and Advanced Inputs
- [ ] 🔴📦 Flake Parts
- [ ] 🔴📦 Flake Utils
- [ ] 🔴📦 FlakeHub

### 07 - Dev Shells and Environments 🟡
- [ ] 🟡🚀 mkShell Basics
- [ ] 🟡🚀 Devshell With Flake
- [ ] 🟡🚀 Multiple Environments
- [ ] 🟡🚀 Direnv and Nix direnv
- [ ] 🟡🚀 Lorri
- [ ] 🟡🚀 Devenv sh
- [ ] 🟡🚀 Environments per Language: Node, Python, Go, Rust
- [ ] 🟡🚀 Cachix devenv
- [ ] 🟡🚀 Sharing Environments With Team

### 08 - nixpkgs 🟡🔴
- [ ] 🟡📦 Nixpkgs Structure
- [ ] 🟡📦 Channels Stable Unstable
- [ ] 🟡📦 Searching on Search NixOS Org
- [ ] 🟡📦 Pkgs By Name
- [ ] 🟡📦 override and overrideAttrs
- [ ] 🟡📦 Overlays Introduction
- [ ] 🔴📦 Overlays Advanced: final and prev
- [ ] 🔴📦 NUR: Nix User Repository
- [ ] 🔴📦 Contributing To nixpkgs
- [ ] 🔴📦 Backports and Cherry Picks

### 09 - NixOS 🟡🔴
- [ ] 🟡🖥️ NixOS Key Concepts
- [ ] 🟡🖥️ Configuration Nix Structure
- [ ] 🟡🖥️ Hardware Configuration Nix
- [ ] 🟡🖥️ NixOS Modules
- [ ] 🟡🖥️ Systemd Services
- [ ] 🟡🖥️ Users and Groups
- [ ] 🟡🖥️ Declarative Networking
- [ ] 🔴🖥️ Filesystems and Disks
- [ ] 🔴🖥️ Bootloader Grub Systemd Boot
- [ ] 🔴🖥️ NixOS Rebuild Switch Test Boot
- [ ] 🔴🖥️ OS Rollbacks and Generations
- [ ] 🔴🖥️ NixOS With Flakes
- [ ] 🔴🖥️ Secrets in NixOS
- [ ] 🔴🖥️ NixOS on Raspberry Pi
- [ ] 🔴🖥️ NixOS on WSL2

### 10 - Home Manager 🟡🔴
- [ ] 🟡🏠 What Is Home Manager
- [ ] 🟡🏠 Standalone Installation
- [ ] 🟡🏠 Installation As NixOS Module
- [ ] 🟡🏠 Home Nix Structure
- [ ] 🟡🏠 Managing User Packages
- [ ] 🟡🏠 Dotfiles With Home Manager
- [ ] 🟡🏠 Shell Bash Zsh Fish
- [ ] 🟡🏠 Git Config
- [ ] 🟡🏠 Neovim Vim
- [ ] 🟡🏠 Tmux and Multiplexers
- [ ] 🔴🏠 Gui Programs
- [ ] 🔴🏠 Home Manager With Flakes
- [ ] 🔴🏠 Custom Hm Modules
- [ ] 🔴🏠 Home Manager Without NixOS

### 11 - nix-darwin 🟡🔴
- [ ] 🟡🍎 What Is Nix Darwin
- [ ] 🟡🍎 Installation
- [ ] 🟡🍎 Darwin Configuration Nix
- [ ] 🟡🍎 Homebrew With Nix Darwin
- [ ] 🟡🍎 Launchd Services
- [ ] 🟡🍎 Macos Defaults
- [ ] 🔴🍎 Nix Darwin With Flakes
- [ ] 🔴🍎 Nix Darwin and Home Manager Together
- [ ] 🔴🍎 Updating and Rollback

### 12 - NixOS Module System 🔴🔵
- [ ] 🔴🖥️ What Is the Module System
- [ ] 🔴🖥️ Options and Config
- [ ] 🔴🖥️ Types in Modules
- [ ] 🔴🖥️ Imports
- [ ] 🔴🖥️ mkIf, mkMerge, mkForce
- [ ] 🔴🖥️ Writing Your Own Module
- [ ] 🔴🖥️ Reusable Modules
- [ ] 🔴🏠 Modules For Home Manager
- [ ] 🔵🖥️ Modules For NixOS
- [ ] 🔵🖥️ Testing Modules

### 13 - Packaging Software 🔴
- [ ] 🔴📦 Packaging C Cpp
- [ ] 🔴📦 Packaging Python
- [ ] 🔴📦 Packaging Node
- [ ] 🔴📦 Packaging Go
- [ ] 🔴📦 Packaging Rust: naersk and crane
- [ ] 🔴📦 Packaging Java
- [ ] 🔴📦 Packaging Electron Apps
- [ ] 🔴📦 Packaging Fonts
- [ ] 🔴📦 Private Packages With Overlays
- [ ] 🔴📦 buildFHSEnv Compatibility Layer

### 14 - CI/CD and Builds 🔴
- [ ] 🔴🚀 Nix in GitHub Actions
- [ ] 🔴🚀 Nix in GitLab CI
- [ ] 🔴🚀 Cachix in CI
- [ ] 🔴🚀 Self Hosted Binary Cache
- [ ] 🔴🚀 Nix Remote Builds
- [ ] 🔴🚀 Hydra Native Nix CI
- [ ] 🔴🚀 Garnix
- [ ] 🔴🚀 Hercules CI

### 15 - Multi-Machine Deployment 🔴🔵
- [ ] 🔴🚀 NixOS Rebuild Remote
- [ ] 🔴🚀 Colmena
- [ ] 🔴🚀 NixOps 4
- [ ] 🔴🚀 Morph
- [ ] 🔴🚀 Deploy Rs
- [ ] 🔵🚀 Krops
- [ ] 🔵🚀 Deployment Tools Comparison

### 16 - Nix in Containers and Cloud 🔴🔵
- [ ] 🔴🚀 NixOS Native Containers
- [ ] 🔴🚀 Docker Images With Nix
- [ ] 🔴🚀 dockerTools.streamLayeredImage
- [ ] 🔴🚀 Minimal OCI Images
- [ ] 🔴🚀 NixOS on AWS Ec2
- [ ] 🔴🚀 NixOS on GCP
- [ ] 🔴🚀 NixOS on Azure
- [ ] 🔴🚀 NixOS on Hetzner
- [ ] 🔴🚀 NixOS on Digital Ocean
- [ ] 🔵🚀 NixOS on Kubernetes
- [ ] 🔵🚀 Nix and Terraform

### 17 - Secrets Management 🔴
- [ ] 🔴🚀 The Secrets Problem in Nix
- [ ] 🔴🚀 Agenix
- [ ] 🔴🚀 Sops Nix
- [ ] 🔴🚀 Ragenix
- [ ] 🔴🚀 Vault With NixOS
- [ ] 🔴🏠 Secrets in Home Manager

### 18 - Ecosystem Tooling 🟡🔴
- [ ] 🟡📦 nix-output-monitor (nom)
- [ ] 🟡📦 nix-index and nix-locate
- [ ] 🟡📦 Comma: Run Any Binary
- [ ] 🟡📦 Alejandra Formatter
- [ ] 🟡📦 Nixfmt
- [ ] 🟡📦 Statix Linter
- [ ] 🟡📦 Deadnix
- [ ] 🟡📦 nvd: Generation Diff
- [ ] 🟡📦 Nix Tree
- [ ] 🟡📦 Nix Du
- [ ] 🟡📦 Manix: Documentation Search
- [ ] 🟡📦 nh: Nix Helper
- [ ] 🔴🖥️ Disko: Declarative Disk Partitioning

### 19 - Patterns and Architecture 🔴🔵
- [ ] 🔴🚀 Structure of a Mature Nix Repo
- [ ] 🔴🚀 Modular vs Monolith
- [ ] 🔴🚀 Flake Parts Advanced
- [ ] 🔴🚀 STD (Standard) and Hive
- [ ] 🔴🚀 Paisano
- [ ] 🔵🚀 Managing Multiple Hosts
- [ ] 🔵🚀 Managing Multiple Users
- [ ] 🔵🚀 Shared Configurations
- [ ] 🔵🚀 Public Dotfiles on GitHub

### 20 - Emerging and New 🔵
- [ ] 🔵📦 Lix Nix Fork
- [ ] 🔵📦 TVix: Rust Reimplementation
- [ ] 🔵🗣️ Official Nix Language Evolution (2026)
- [ ] 🔵📦 FlakeHub and the Commercial Ecosystem
- [ ] 🔵📦 Placeholder: New Topic


---

## Recommended resources

- [NixOS & Flakes Book](https://nixos-and-flakes.thiscute.world/) — best free book to start
- [Official Nix Manual](https://nixos.org/manual/nix/stable/)
- [NixOS Wiki](https://wiki.nixos.org/)
- [nixpkgs Manual](https://nixos.org/manual/nixpkgs/stable/)
- [Home Manager Manual](https://nix-community.github.io/home-manager/)
- [nix.dev](https://nix.dev/) — official tutorials
- [Zero to Nix](https://zero.to-nix.com/) — by Determinate Systems
- [search.nixos.org](https://search.nixos.org/) — package and option search
- [Nixpkgs PR tracker](https://nixpk.gs/pr-tracker.html)
- [FlakeHub](https://flakehub.com/) — flake discovery platform

---

## 20 — Emerging & New

> This is a living category. As new tools, forks, RFCs, or ecosystem shifts emerge during your
> study period, they will be added here as new subfolders. Particularly worth watching in 2026:
> **Lix** (the community Nix fork), **TVix** (Nix reimplemented in Rust by the Tvix team),
> and any changes to the official Flakes stabilization process.
