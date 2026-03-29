---
title: Getting Started
tags:
  - guide
  - setup
---

# Getting Started

## How to Add Notes

1. Create `.md` files in the `content/` folder
2. Add frontmatter (title, tags, etc.) at the top of each file
3. Use Obsidian-style wikilinks: `[[page-name]]`
4. Commit and push to trigger auto-deployment

## Folder Structure

```
content/
├── index.md          # Homepage
├── getting-started.md # This page
├── notes/            # Your notes folder
│   ├── note-1.md
│   └── note-2.md
└── ...
```

## Supported Syntax

### Wikilinks

- `[[page-name]]` - Link to another page
- `[[page-name|Display Text]]` - Link with custom text
- `[[page-name#heading]]` - Link to a specific heading

### Tags

Add tags in frontmatter:

```yaml
---
tags:
  - tag1
  - tag2
---
```

### Callouts

> [!note]
> This is a callout, just like in Obsidian!

> [!tip]
> You can use all Obsidian callout types: note, tip, warning, danger, etc.

## Local Development

```bash
npx quartz build --serve
```

This starts a local server at `http://localhost:8080` for previewing your site.
