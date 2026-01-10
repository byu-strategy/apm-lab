# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Quarto book project for **STRAT 477R – Associate Product Manager Lab**, a for-credit, apprenticeship-style internship program at BYU. The site serves two audiences: students completing APM internships and partner companies hosting interns.

## Build Commands

- **Preview during development**: `quarto preview` (primary local workflow)
- **Check Quarto installation**: `quarto --version`

**Note**: Never render locally. The site auto-renders via GitHub Actions when pushed to main. See `.github/workflows/publish.yml`.

The GitHub workflow renders the site and deploys to GitHub Pages. Output goes to `docs/` directory.

## Content Structure

### Site Organization
```
index.qmd                    # Program overview (dual-audience landing page)
schedule.qmd                 # Key dates and deadlines

students/                    # Student-facing content
  01-syllabus.qmd            # Grading, policies, BYU boilerplate
  02-getting-started.qmd     # Onboarding, expectations, first week checklist
  03-weekly-updates.qmd      # Weekly email format, examples, deadlines
  04-pm-skills.qmd           # Product management skills and resources

partners/                    # Company partner-facing content
  01-program-overview.qmd    # Structure, hours, credit, timeline
  02-working-with-interns.qmd # Setting goals, check-ins, mentoring
  03-evaluation.qmd          # End-of-term feedback survey, wrap-up
  04-faq.qmd                 # Equipment, HR, paperwork, extensions
```

### Dual Audience Focus
- **Students**: Interns earning academic credit through real product work
- **Company Partners**: Companies hosting and mentoring APM interns

## Quarto Configuration

Key settings in `_quarto.yml`:
- **Type**: Book project outputting to `docs/`
- **Theme**: Cosmo with custom CSS (`styles.css`)
- **Structure**: Organized into "For Students" and "For Partners" parts

## Development Notes

- Images stored in `images/` directory
- Custom styling through `styles.css`
- Header and footer templates in `_header.html` and `_footer.html`

## Program Context

- **Duration**: 4 months (January 7 – April 15, 2026)
- **Hours**: 10-20 hours/week
- **Credit**: 3.0-6.0 credit hours
- **Key deliverable**: Weekly progress emails (due Saturday 11:59 PM)
- **Evaluation**: Mentor feedback survey at end of term
