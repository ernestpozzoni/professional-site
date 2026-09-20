# Repository Notes

This repository is the portable content source for the GitBook professional-site prototype.

## Design rules

- GitBook is the presentation layer; this repository is the durable content layer.
- Essential content must remain readable as ordinary Markdown.
- Internal page links use relative paths.
- Filenames are lowercase and hyphenated where practical.
- `SUMMARY.md` records navigation order.
- Essential information must not exist only inside GitBook-specific blocks.
- Article and project classifications must also be stored in each Markdown file as plain-text YAML front matter; GitBook-native tags are supplementary only.
- Original media and source documents are stored separately from page text.
- PDF files are reference outputs, not the editable master of the site.
- Public GitBook URLs are recorded separately in `migration/url-inventory.md`.

## Prototype scope

The prototype contains:

1. CV homepage
2. Portfolio overview
3. One representative detailed project
4. CV-to-project relative link
5. Articles and Publications overview
6. One prototype original article
7. One external-publication record template
8. Speaking and Facilitation page
9. Contact page
10. `SUMMARY.md`

## Source files

- `assets/documents/cv-2026-08-24.pdf`
- `assets/documents/project-portfolio-2026-08-24.pdf`

The Markdown pages are the migration-test content; the PDFs are preserved only as reference outputs.
