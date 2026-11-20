# Project Milestone – Accessibility and Visual Design

This portfolio includes a Home page (`index.html`), Projects page (`project.html`), and About/Contact page (`about.html`).

## 1. Accessibility improvements

Initial WAVE screenshots reported one missing-language error and four contrast errors on Home, and one missing-language error, one missing form-label error, and six contrast errors on About.

- Added `lang="en"` to the Home page HTML element to identify the document language for screen readers.
- Added `lang="en"` to the About page HTML element to identify the document language for screen readers.
- Replaced white body text on a white background with dark text on a light background to improve readability across the shared stylesheet.
- Restored the shared light background so content and text use a consistent, readable palette across the pages.
- Removed the unlabelled name input from the About page's goals section and replaced it with a properly labelled name field in the contact form.
- Fixed the broken Home navigation link by setting the Projects link destination to `project.html`.
- Added visible keyboard-focus indicators for the contact inputs, textarea, and submit button.

## 2. Visual design: Gestalt principles

- **Proximity:** Project titles, descriptions, and links are grouped together within bordered project cards, and related contact inputs are grouped in a fieldset.
- **Similarity:** Navigation links and blue action buttons share matching styles across the portfolio pages.
- **Consistent palette:** Shared CSS variables provide navy headings and headers, blue action buttons, dark body text, and light backgrounds on all three pages.

## 3. Accessible contact form

- Added a contact form to the About page with name, email, and message fields.
- Associated each visible `label` with its input using matching `for` and `id` attributes.
- Grouped name and email under a `fieldset` with a descriptive `legend`.
- Added field-specific validation errors, `aria-invalid`, `aria-describedby`, and live announcements to explain invalid submissions.
- The form prepares a `mailto:` email in the visitor's email app; it does not send or save messages through a website server.

## 4. Testing notes

- WAVE was previously run on the Home and About pages, with issues recorded above.
- The Projects page and all three updated pages still need a fresh WAVE run to verify that the final deployed site has zero accessibility errors.
- Shared design colors were selected for WCAG AA contrast; verify all rendered combinations using [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) and WAVE.
