# QUBITS AI AUŠRA

QUBITS AI AUŠRA is a digital publishing project built around the central book publication: a critical and editorial exploration of the qubit, intelligence, and the future of human-machine collaboration.

## Project identity

- Title: QUBITS AI AUŠRA
- Subtitle: De onde veio o qubit — e para onde ele pode levar a inteligência?
- Editorial manifesto: AUTOMATIZE A TAREFA. AMPLIFIQUE A PESSOA.

## What this repository contains

This repository is organised as a professional editorial publication site and archive. It preserves the project's intellectual and editorial materials while creating a clear digital publishing structure for the public website, book access, documentation, and repository audit.

## Book location

The primary publication asset is the PDF in the book directory:

- `book/QUBITS_AI_AUSRA_full.pdf`

The public website links to this file as the canonical book access point.

## Website and GitHub Pages

The repository root `index.html` is the public landing page for the project. It is intended for GitHub Pages deployment and built as a static, responsive editorial website.

GitHub Pages is configured through a GitHub Actions workflow at:

- `.github/workflows/pages.yml`

The repository uses the GitHub Pages deployment workflow rather than the default branch-only static hosting pattern because the project is structured as a publication site and should be deployed through the supported Actions pipeline.

## Editorial materials

The editorial documents are preserved and organised into this structure:

- `editorial/README.md`
- `editorial/manifesto.md`
- `editorial/editorial-policy.md`
- `editorial/methodology.md`
- `editorial/about.md`

## Book and publication structure

- `book/README.md`
- `book/manuscript/README.md`
- `book/editions/README.md`
- `book/metadata/README.md`

## Audit and change tracking

- `audit/change-log.md`
- `audit/repository-audit.md`

## Documentation

- `docs/README.md`
- `docs/publication.md`

## Publication status

This repository is in a finalised publishing preparation state:

- production landing page is in place
- book PDF is accessible from the website
- editorial and audit documentation is organised
- GitHub Pages deployment workflow is prepared

## Repository structure

```text
/
├── index.html
├── README.md
├── book/
├── editorial/
├── audit/
├── docs/
├── web/
├── .github/
└── ...
```

## Change tracking

The authoritative repository change log is maintained in `audit/change-log.md` and should be used as the reference for project evolution and final publication preparation.
