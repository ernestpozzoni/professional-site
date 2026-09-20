# Prototype Acceptance Test

Run this test **after Git Sync is configured and the GitBook prototype has been published**.

## 1. Repository independence

- [ ] Clone the repository into a new local directory.
- [ ] Confirm that no GitBook workspace access is required to read the files.
- [ ] Confirm that `README.md`, `SUMMARY.md`, portfolio, article, speaking and contact pages are present.

## 2. Markdown readability

- [ ] Open every `.md` file in a plain text editor.
- [ ] Confirm that all essential information is intelligible without GitBook.
- [ ] Confirm that no essential information exists only in a proprietary GitBook block.

## 3. Internal links

- [ ] From `README.md`, follow the link from the Link Communications Systems entry to the representative case study.
- [ ] From `portfolio/README.md`, follow the case-study link.
- [ ] From the sample article, follow the related-case-study link.
- [ ] Confirm that links work from the cloned repository or another Markdown renderer.

## 4. Navigation

- [ ] Open `SUMMARY.md`.
- [ ] Confirm that the intended navigation order is explicit.
- [ ] Compare the GitBook navigation with `SUMMARY.md`.

## 5. Media and files

- [ ] Confirm that both reference PDFs are present under `assets/documents/`.
- [ ] Add any future images as repository files rather than GitBook-only assets wherever practical.
- [ ] Confirm that repository-relative media links still resolve after cloning.

## 6. Cross-renderer test

Render or browse the repository using at least one substantially different Markdown-compatible tool, such as GitHub/GitLab’s repository renderer or a local Markdown/static-site tool.

- [ ] Pages remain readable.
- [ ] Relative links still make sense.
- [ ] Headings and lists remain intelligible.
- [ ] Essential information does not depend on GitBook styling.

## 7. Reconstruction test

Using only:

- the cloned repository,
- the independent media/document backup, and
- the URL inventory,

attempt to reconstruct the page hierarchy in another Markdown-compatible system.

- [ ] No page must be manually copied out of GitBook.
- [ ] No relationship between CV, portfolio and articles must be recreated from memory.
- [ ] Navigation order can be reconstructed from `SUMMARY.md`.

## 8. URL inventory

- [ ] Populate `migration/url-inventory.md` with every actual GitBook public URL.
- [ ] Record the personal domain forwarding target.
- [ ] Preserve the inventory in every backup.

## Decision

**PASS:** Continue migration of the remaining CV-linked projects and articles.  
**CORRECTABLE:** Fix filenames, relative links, media handling, Markdown structure or GitBook-block usage and repeat the test.  
**FAIL:** Reconsider GitBook only if the underlying content or page relationships cannot be preserved.
## 9. Tag and category portability

- [ ] Open each project and article Markdown file.
- [ ] Confirm that categories and tags are recorded in plain-text YAML front matter.
- [ ] Confirm that no classification exists only as a GitBook-native tag.
- [ ] Confirm that another Markdown-compatible system could reconstruct the page-to-tag relationship without relying on memory.

