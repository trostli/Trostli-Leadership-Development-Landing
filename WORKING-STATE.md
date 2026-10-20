# TLD website working state

Last updated: 2026-10-20

## Current status

The approved Option 2 English website is live on `main` and served at:

https://trostlileadership.com

The public contact page is:

https://trostlileadership.com/contact.html

The working tree is clean. The previous website remains preserved in the archive
branch `archive-old-website-2026-10-19`.

## Repository and branches

- Repository: https://github.com/trostli/Trostli-Leadership-Development-Landing
- Local repository: `/Users/trostli/Documents/GitHub/Trostli-Leadership-Development-Landing`
- Production branch: `main`
- Current production commit: `489965e`
- Revision branch: `feature/tld-revision`
- Archive branch: `archive-old-website-2026-10-19`

The local `main` branch must be synchronized before starting new work. Never rewrite
production history or delete the archive branch.

## Approved design

Option 2 is the approved design. It uses the navy, white, charcoal, and gold palette;
the leadership-transition hero; the Book a Discovery Call, Learn More, and Get in Touch
CTAs; the Who We Serve and How We Can Work Together sections; the About Carlos section;
organizational leadership support; thoughtful first-step and good-fit content; and the
footer contact and certification details.

The How I Work section uses three white cards with gold circular icon medallions:
Strategic Clarity, Leadership Presence, and Trusted Relationships. The safe and
confidential space phrase has a gold underline. On mobile, the sticky header is 68px,
the logo is 28px, and anchored sections reserve 84px of scroll offset.

Option 1 was reviewed during the design process and retained as a possible future
alternative. It is not the approved live design. Do not infer its implementation
details without the original reference.

## Completed implementation history

- PR #1 implemented the main approved website revision and was merged into `main`.
- PR #2 implemented mobile homepage refinements, including improved hero spacing and
  CTA visibility. The relevant commit is `afe7efb`.
- PR #3 implemented the compact mobile header and scroll offset. The relevant commit is
  `1abf8ff`; the merge commit is `70a7896`.
- PR #4 refreshed this handoff file. The content commit is `cf99728`; the merge commit is
  `8fb2274`.
- PR #5 completed the approved accessibility fixes: accessible names for the WhatsApp and
  LinkedIn icon links, decorative duplicate carousel logos, reduced-motion support, and the
  corrected credibility-section heading level. The content commit is `9e722e6`; the merge
  commit is `489965e`. The six organization logos remain unchanged by approval.
- The live homepage, contact page, Google Form embed, Calendly links, phone, email,
  LinkedIn, and WhatsApp links were smoke-tested.

## External integrations

- Calendly: https://calendly.com/trostlileadership/executive-consultation
- Google Form: https://docs.google.com/forms/d/e/1FAIpQLSfGk9v7VcVJ6HzXlvkpLftBoFVPKVTgQILHHz_uuAoVVoIFtA/viewform
- Phone: +1 (617) 800-9181
- Email: trostli@trostlileadership.com
- LinkedIn: https://www.linkedin.com/in/ctrostli/
- WhatsApp: https://wa.me/12016966020

The Google Form accepts public responses without Google sign-in. The response flow was
tested, and the test response was deleted. The linked Google Sheet destination has not
been verified. Do not guess or record a Sheet URL until it is confirmed.

PostHog is loaded on the live site and CTA click tracking exists. Review and confirm
that tracking before extending it. Do not record the project key or any credentials.

## Hosting

The site uses GitHub Pages with the custom domain `trostlileadership.com`, represented
by the repository `CNAME` file. No `.github/workflows` deployment workflow exists.
The GitHub Pages source branch and folder setting have not been independently verified.
Allow for GitHub Pages caching after merges.

## Future GitHub workflow

1. Synchronize local `main` with origin.
2. Create or use a clearly named revision branch.
3. Inspect the relevant files and current diff.
4. Make only the approved change.
5. Run `git diff --check`.
6. Review the complete diff.
7. Commit with a descriptive message.
8. Push the revision branch.
9. Create a pull request into `main`.
10. Review the pull request diff and checks.
11. Merge only after Carlos approves.
12. Verify the live site after the merge.
13. Record the commit, pull request, merge, and verification details here and in
    `02_Projects/TLD Web Page Improvements.md`.
14. Keep the archive branch intact.

## QA checklist

After future changes, check desktop and narrow mobile layouts; the hero, About Carlos,
Who We Serve, How I Work, How We Can Work Together, organizational support, thoughtful
first-step, good-fit, final CTA, and footer sections; all Calendly, contact, phone,
email, LinkedIn, WhatsApp, logo, and internal anchor links; the Google Form submission
and confirmation flow; heading structure, alt text, contrast, keyboard focus, tap-target
size, console errors, and broken links.

## Deferred post-launch work

These are improvements, not launch blockers:

1. Add approved testimonials or reviews. A hidden placeholder exists, but public proof
   requires Carlos's approval and permission.
2. Complete a deeper accessibility and link review.
3. Review and confirm the existing PostHog CTA tracking, then extend it if needed.
4. Consider replacing the Tailwind CDN with a production CSS build.

The culturally adapted Brazilian Portuguese version remains future work after the English
page is intentionally approved.

## Resume instruction

When continuing after a break, read this file, then read `CLAUDE.md` and the relevant
CDT_PKA project record. Verify `git status --short --branch`, synchronize `main`, inspect
the current diff, and check GitHub before assuming work is unfinished. Do not repeat the
completed implementation history. Start with the first approved unfinished item, propose
significant changes before editing, and use the GitHub workflow above.
