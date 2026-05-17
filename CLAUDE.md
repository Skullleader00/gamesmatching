# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a Blogger template (`game matching.xml`) for "Game Matching" - a Thai card game hub covering Cardfight!! Vanguard, Yu-Gi-Oh! Master Duel, and Shadowverse: World Beyond. The template displays meta decks, tier lists, and game information in Thai language.

## Architecture

The template uses Blogger's XML templating system with the following key components:

### Content Structure
- **Homepage** (`data:blog.pageType == "index"`): Displays hero section, tier lists, game hub cards, and weekly meta decks
- **Post pages**: Shows individual blog posts with comments via Blogger's built-in widgets

### Data-Driven Sections
- **Featured decks**: Posts tagged with `meta-deck-recommended`
- **Latest decks**: Posts tagged with `meta-deck-latest`
- **Game sections**: Posts tagged with `Vanguard`, `YuGiOh`, `Shadowverse`, or `Meta`

### Styling System
All styles are embedded in `<b:skin><![CDATA[...]]></b:skin>` with:
- CSS custom properties for colors (blue, pink, red accents for different games)
- Responsive grid layouts using CSS Grid and Flexbox
- Tier colors: pink (S-tier), blue (A-tier), red (B-tier)

## Editing Workflow

1. **Test template changes**: Upload to Blogger and verify rendering
2. **Validate XML syntax**: Ensure all tags are properly closed
3. **Check mobile responsiveness**: Test at 768px breakpoint
4. **Verify label filtering**: Confirm posts appear under correct sections based on labels