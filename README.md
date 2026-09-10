# Counterform

**An AI-powered Chrome extension that automates job application forms.**

Counterform reads a job application form directly from the page, reasons
about which fields need what, and fills them in. It primarily watches for resume/CV
uploads, custom-styled dropdowns and comboboxes (React-Select and
similar libraries), Yes/No toggle questions, and multi-step ATS
platforms like Ashby, Greenhouse, and Lever.

This repository is intentionally a placeholder. Counterform's source is
closed while it's under active development toward a commercial release.
This page exists to describe what the project does, for anyone curious,
without publishing the implementation.

## What it does

- Scans the current page's DOM - including embedded iframes some ATS
  platforms render the actual form inside - to find every actionable
  field
- Uses an LLM to decide what to fill, what to skip, and what to leave
  for the user to answer themselves. Open-ended or subjective questions
  are never auto-answered; the user gets an AI-drafted suggestion to
  review and edit instead
- Handles file uploads (resume, cover letter, etc.) by matching a
  human-readable name to the right field
- Drives complex custom UI widgets - searchable comboboxes, custom
  Yes/No toggles - the way a real user would, not just by writing
  values into the DOM
- Never auto-submits an application. The user always reviews the
  completed form and clicks Submit themselves

## Status

Actively developed. Not yet published to the Chrome Web Store —
link coming soon.

## Get in touch

www.linkedin.com/in/kenneth-snyder-83ab45360
