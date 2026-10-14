# Paper Manager

### A TUI research paper manager written in rust

### TUI
|--------------------------------|
|          |                     |
|          |                     |
|          |                     |
| Keywords |                     |
|          |                     |
|   tags   | Main List of papers |
|          |                     |
|  filters |                     |
|          |                     |
|          |                     |
|--------------------------------|
|       Search (VIM-like)        |
|--------------------------------|

### Local Data Structure
Files:
- index.sqlite
- references.bib
- config.toml

Folders:
- notes
- pdfs


### Features
- nucleo crate and SQlite FTS5 for searching
- vim bindings
- bibtex management
- create key based on bibtex import, pdf named <key>.pdf, note named <key>.md
- tags
- notes in markdown, linked to entries
- auto-category and manual category (say having references for a specific paper separate)
- duplicate detection
- import/export bibtex
- open pdfs with external viewer
- entries do not require a pdf
- master bib is source of truth, keep on github, index can be rebuilt from it
- in master bib, save tags, keywords, etc. as extra fields

### Optional Later Features
- GROBID for metadata extraction
- related paper matching (direct references, fuzzy, etc.)
- in-pdf links to local references?
