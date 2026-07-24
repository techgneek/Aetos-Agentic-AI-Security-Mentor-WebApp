# Publishing Process

This page explains how the public documentation is organized.

Return to the [Documentation Index](index.md).

## Public Repo Goal

The public repository is meant to be a clean markdown-only view of the project story.

It should be easy to browse, safe to share, and separate from the private implementation repository.

## Organization

- `README.md` serves as the public entry point.
- `docs/` contains the supporting markdown pages.
- Links inside the public repo should point to other markdown pages or the live site.

## What To Avoid

- source code
- private repo links
- internal API route references
- deployment internals
- private automation or secret-management instructions

## Maintenance Rule

If a page needs to mention something technical, keep it at the product-story level and avoid implementation-specific details.