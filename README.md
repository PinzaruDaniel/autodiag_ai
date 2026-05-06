# Autodiag AI

Autodiag AI is a multi-repository project that pairs a backend service with a Flutter client. This repository acts as the workspace that ties those components together via git submodules.

## Repository structure

- `src/backend` — backend service (submodule: `autodiag_backend`)
- `src/flutter` — Flutter client app (submodule: `autodiag_flutter`)

## Getting started

### Prerequisites

- Git

### Clone with submodules

```bash
git clone --recurse-submodules https://github.com/PinzaruDaniel/autodiag_ai.git
```

If you already cloned the repository:

```bash
git submodule update --init --recursive
```

### Set up each component

Each submodule contains its own README with detailed setup, dependencies, and run instructions:

- `src/backend/README.md`
- `src/flutter/README.md`

## Working with submodules

Update submodules to the latest referenced commits:

```bash
git submodule update --remote --merge
```

When making changes inside a submodule, commit there first, then commit the updated submodule pointer in this repository.

## Contributing

1. Create a feature branch.
2. Make changes in the relevant submodule(s).
3. Update this repository to point to the new submodule commits.
4. Open a pull request with a clear description of the changes.
