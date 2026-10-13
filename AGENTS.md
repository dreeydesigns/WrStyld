# STYLD Agent Constitution

Project: STYLD, a trust-first beauty marketplace for Kenya. Roles: Client, Professional, Salon, Shop, Delivery, Admin.
Launch scope: Client, Professional, Salon only. Shop and Delivery stay disabled (interest register only).
Auth: Better Auth, one identity, many workspaces. Do not add or reintroduce any other auth provider. Do not touch Clerk configuration.
Brand: keep the approved STYLD logo artwork exactly (Logo Book). Never recreate the logo with a font or redraw it.

## Design system (source of truth: STYLD Design System .ds file and app/globals.css)
- Palette: Ink #1D1D1B (text, primary CTA background), Clay #C0A090 (selected, premium accents, never body text on light surfaces), Clay text #875945 (accessible clay for text and links), Sage #909888 (supporting and informational states), Canvas #FAF8F5 (page background), White #FFFFFF (cards).
- Primary CTA: Ink background with white text. Secondary: white or canvas with Ink border and Ink text. Selected chips and tabs: Clay.
- Do not use purple, violet, blush, rose or pink treatments anywhere, including Tailwind purple-*, violet-*, pink-*, rose-* classes and hex values such as #8B5CF6, #C2707A, #1A1A2E.
- Use the CSS variables in app/globals.css. Do not hardcode hex colours in components. New tokens go in app/globals.css only.
- Type: Playfair Display for display headings, DM Sans for UI and body, Great Vibes for at most one accent word per page.
- Icons: Lucide outline. No emoji as icons.
- Text contrast must meet WCAG 2.2 AA (4.5:1 normal text, 3:1 large text and UI parts).
- Motion: transform and opacity only, respect prefers-reduced-motion, never block content behind a splash or animation.
- Imagery: licensed or approved photography only. If an image is missing, use the neutral branded placeholder and report the photo needed.

## Hard rules
- Work only on the test branch. Never push to main, never force-push, never deploy to Production, never merge.
