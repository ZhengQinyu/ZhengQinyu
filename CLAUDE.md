# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a GitHub Profile README repository for user imknn (KN郑某某). It renders as the user's public GitHub profile page.

## Structure

- `README.md` - The main profile page with personal info, tech stack badges, contribution graph, and blog posts
- `.github/workflows/snake.yml` - GitHub Actions workflow that generates an animated snake SVG from the contribution graph using [Platane/snk](https://github.com/Platane/snk)

## Workflow Details

The snake animation workflow:
- Runs every 24 hours on schedule, on push to main, or manually via workflow_dispatch
- Outputs SVGs to the `output` branch (not main)
- Uses `Platane/snk/svg-only@v3` with palette options for light and dark themes
- Generated SVGs are referenced from `raw.githubusercontent.com` on the `output` branch

## Notes

- Blog post list is maintained manually between `BLOG-POST-LIST:START` and `BLOG-POST-LIST:END` markers in README.md
- Shield.io badges use `style=for-the-badge` for consistent large badge styling
- The profile targets both light and dark GitHub themes with separate snake SVG variants
