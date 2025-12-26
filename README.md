# Certificates

A curated collection of certificates for courses, workshops, and training I've completed. This repository is a single place to store, organize, and showcase verifiable proof of learning.

Repository: [DishiGpt/Certificates](https://github.com/DishiGpt/Certificates)

---

## Table of contents

- [Purpose](#purpose)
- [Structure](#structure)
- [How to browse the certificates](#how-to-browse-the-certificates)
- [How to add a new certificate](#how-to-add-a-new-certificate)
- [Naming & metadata conventions](#naming--metadata-conventions)
- [Automation & publishing ideas](#automation--publishing-ideas)
- [Privacy and security](#privacy-and-security)
- [License](#license)
- [Contact](#contact)

---

## Purpose

This repo is intended to:
- Keep all course and certification documents in one version-controlled place.
- Provide a simple, consistent structure so certificates are easy to find and verify.
- Make it straightforward to share a persistent public index (for example via GitHub Pages) when needed.

---

## Structure

Suggested repository layout (example):

- certificates/
  - provider-name/
    - 2024-05-coursera-machine-learning.pdf
    - 2024-05-coursera-machine-learning.md  (metadata + optional notes)
  - udemy/
    - 2023-11-udemy-react-basics.pdf
- index.yml (optional — machine-readable index of all certificates)
- README.md

Organize by provider (Coursera, Udemy, edX, company-training, etc.) or by year — pick whichever is easiest for you and keep it consistent.

---

## How to browse the certificates

- Use the repository tree on GitHub to navigate providers and years.
- If you add an `index.yml` or `index.json` file, you can generate a webpage (GitHub Pages) that lists them automatically.
- Add short markdown files alongside each certificate (e.g., `*.md`) with context: course summary, skills learned, and a link to the issuing page (if available).

---

## How to add a new certificate

1. Create or navigate to the appropriate folder, e.g. `certificates/coursera/`.
2. Add the certificate file (PDF, image) following the naming convention below.
3. Add a small metadata Markdown file with details (sample below).
4. (Optional) Update `index.yml` with the new record.

Sample steps:
- filename: `2025-02-coursera-deep-learning.pdf`
- metadata file: `2025-02-coursera-deep-learning.md` (or `.yml`)

A metadata template you can copy:

```markdown
---
title: "Deep Learning Specialization"
provider: "Coursera"
date_awarded: "2025-02-10"
certificate_file: "2025-02-coursera-deep-learning.pdf"
credential_id: "ABC-123-XYZ" # optional
credential_url: "https://www.coursera.org/account/accomplishments/verify/ABC-123-XYZ" # optional
skills:
  - "Neural Networks"
  - "CNN"
  - "Sequence Models"
notes: |
  Short notes about what you learned, project highlights, or lab work.
---
```

---

## Naming & metadata conventions

Consistent names help indexing and automation. Suggested filename pattern:

YYYY-MM-provider-short-title.ext

Examples:
- `2024-11-udemy-react-basics.pdf`
- `2023-07-coursera-data-science.md`

Metadata fields to include (in YAML front-matter or an `index.yml`):
- title
- provider
- date_awarded
- certificate_file
- credential_id (if any)
- credential_url (verifiable link)
- tags/skills

---

## Automation & publishing ideas

- Add an `index.yml` or `certificates.json` that lists every certificate and includes metadata. This makes it easier to:
  - Auto-generate a human-readable gallery page with GitHub Pages.
  - Build a small script to create a living CV / portfolio page.
- Use GitHub Actions to:
  - Validate new PRs follow naming/metadata conventions.
  - Regenerate an HTML index when the repository changes.
- Use an RSS feed or a pinned README section to highlight newest certificates.

If you'd like, I can provide:
- A GitHub Action to validate and index certificates.
- A simple static site generator template (Jekyll or plain HTML) to publish to GitHub Pages.

---

## Privacy and security

- Certificates often include personal information (full name, email, images). Consider whether you want the repo public.
- If you must keep some certificates private, consider:
  - Creating a private repository.
  - Keeping sensitive documents out of the repo and storing only metadata and verification links publicly.
  - Redacting or converting to images/PDFs that hide personal details you don't want exposed.

---

## License

Include a license if you want others to reuse the organization or tooling. If this repository is just a personal archive, you can leave it unlicensed or add a permissive license such as the MIT License.

---

## Contact

If you want help organizing the repo, adding automation (Actions), or publishing to GitHub Pages, open an issue or create a PR here:
- Repository: [DishiGpt/Certificates](https://github.com/DishiGpt/Certificates)

---

Thank you — congratulations on your learning progress! Keep this repo updated as you complete more courses.
