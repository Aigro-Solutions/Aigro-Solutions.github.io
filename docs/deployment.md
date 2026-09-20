# Deployment

## Current repository state

The production site is a static GitHub Pages publication. The intended workflow is `.github/workflows/pages.yml` and deploys the root `index.html` together with the web, book, editorial, audit, and documentation directories.

## Branch

The workflow is configured for pushes to `AigroQuantumSaas`, the current production branch identified for this repository.

## External GitHub setting

An administrator must ensure that repository Pages is configured to use **GitHub Actions** as its source. This cannot be enforced by a repository file alone.

## Book asset

The current branch audit did not find a PDF. The site therefore does not expose a fabricated download link. When the authorised PDF is supplied, place it at `book/QUBITS_AI_AUSRA_full.pdf` only if that is the actual filename, then add and validate the link in `index.html`.
