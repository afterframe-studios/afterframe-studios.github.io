# AFTERFRAME studios — Website prototype v0.7

Static, responsive, bilingual (Italian/English) website prototype for AFTERFRAME studios.

## Included
- `index.html` — one-page studio website
- `css/styles.css` — responsive visual system
- `js/site.js` — language switch, mobile navigation, and contact message builder
- `assets/img/` — approved brand kit logo exports

## Run locally
Open `index.html` in a modern browser. For a local server, use VS Code Live Server or run `python -m http.server` from this folder.

## Publish with GitHub Pages
1. Create or open the repository for the AFTERFRAME website.
2. Upload the **contents** of this folder to the repository root (so `index.html` is at the root).
3. In GitHub, open **Settings → Pages**.
4. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. Wait for GitHub Pages to publish the site.

## Notes
- No backend, database, account system, or paid service is required.
- Google Fonts are loaded online; if unavailable, system serif/sans-serif fallbacks are used.
- The Stories section intentionally contains no fictional releases. Replace its empty state when the first real story is ready.
- The contact area includes collaboration, press/media, and follow-the-project information, plus a bilingual message builder. The form does not send or store personal data: it prepares text for the visitor to copy. Connect an official email or a backend before enabling actual message delivery. Social links are intentionally omitted until official channels exist.
- This is a first navigable prototype, not yet a final production release.

## Version 0.2 — Contact section
- Expanded contact pathways for collaborations, press/media, and project updates.
- Added a bilingual contact form with required-field validation.
- The form generates a copyable message locally; no information is transmitted or stored.
- Added responsive layout and translated placeholders/status messages.


## Version 0.3 — About chapter
- Expanded the Studio section into a bilingual About chapter built around the studio's founding idea.
- Added the central “what if?” question, the distinction between emotional engagement and narrative agency, and the studio's creative purpose.
- Reframed the three pillars as Cinema, Literature, and Interactivity.
- Added an editorial closing statement that presents AFTERFRAME as an open creative space with room to grow into a team.
- Updated the navigation label to About and added responsive styling for the new chapter.
- The site remains a static, bilingual one-page prototype; no stories, team members, social accounts, or contact addresses have been invented.


## Version 0.4 — Motion language
- Added restrained entrance transitions for the hero and scroll-triggered reveals for key content blocks.
- Added subtle hover feedback to navigation links, contact cards, buttons, the story placeholder mark, and the three creative pillars.
- Added a compact animated mobile-menu icon state and clearer keyboard focus styling.
- Respects the visitor's `prefers-reduced-motion` accessibility setting; content remains visible when motion is unsupported.
- No new external libraries, services, media assets, or interactive story content are required.


## Version 0.5 — cinematic finish
- Refined the typographic hierarchy, spacing, line-height and responsive heading scale for a more cinematic/editorial reading rhythm.
- Added a very subtle full-page film-grain texture while keeping the existing hero treatment restrained.
- Introduced fine bronze section rules and atmospheric background transitions between the main chapters.
- Rebuilt the footer with the approved wordmark, bilingual studio descriptor, section navigation, return-to-top link and copyright line. No unconfirmed social profiles, addresses or contact details were added.
- Checked responsive footer and heading layouts at tablet and mobile breakpoints.
- Preserved bilingual content, keyboard focus, and the existing `prefers-reduced-motion` support.
- The logo animation and any narrative demonstration remain intentionally deferred.


## Anteprima video Hero (temporanea)
La versione include temporaneamente `assets/video/hero-temporary.mp4` nel riquadro della Hero. Il video è impostato in autoplay silenzioso, loop e riproduzione inline. Potrà essere sostituito o rimosso quando sarà pronta la versione definitiva della logo animation.


## Version 0.6 — definitive Hero animation
- Replaced the temporary Hero video with the approved AFTERFRAME brand animation.
- The Hero video is served as a silent H.264 MP4, 1920×1080, 25 fps, approximately 11 seconds, with autoplay, muted, loop and inline playback.
- Kept the existing footer copyright line: `© [current year] AFTERFRAME studios` and the bilingual rights-reserved text. The year is populated dynamically by `js/site.js`.
- Preserved the existing bilingual layout, navigation, contact message builder, responsive styling and accessibility behavior.


## Version 0.6.1 — footer visibility fix
- Excluded the copyright row (`.footer-bottom`) from the scroll-reveal animation so it remains visible independently of the footer animation observer.
- Preserved the copyright year and bilingual rights-reserved text.


## Version 0.7 — final visual refinements
- Translated the Italian Hero headline to “Ci sono storie che restano con te.”; the English headline remains unchanged.
- Centred the Hero video frame on tablet and mobile layouts.
- Unified the colour of the third paragraph in the Italian About introduction with the surrounding body copy.
- Increased the spacing above the introductory paragraph in the Contact section on desktop and refined its line-height on mobile.
- Added a footer-specific official wordmark export with the two short rules beside the payoff removed; the header wordmark remains unchanged.
- Preserved all other approved content and functionality from v0.6.1. No official contact channels or social links were added.


## Version 0.7.1 — desktop Italian Hero headline fix
- Reduced the Italian Hero headline size on desktop only, so “Ci sono storie / che restano con te.” stays within two lines and clear of the video frame.
- Left the English Hero, all mobile/tablet styles, and all other sections unchanged.


## Version 0.7.8 — social sharing metadata
- Added the approved 1200×630 px social preview image at `assets/img/AFTERFRAME_social_preview_1200x630.png`, without altering the original artwork.
- Added Open Graph metadata (title, description, locale, site name, image dimensions and alt text).
- Added Twitter/X `summary_large_image` metadata with matching title, description and image.
- The image metadata currently uses a relative path because the website has not yet been published. After publication, replace both `og:image` and `twitter:image` values with the full absolute public URL of the image.
- No canonical URL or `og:url` has been added because the final public website address is not yet established.
- Preserved the existing page content, styling, scripts, favicons, video and responsive behavior.


## Version 0.7.9 — accessibility refinements
- Added a skip-to-content link and a clearer keyboard focus indicator.
- Added bilingual accessible labels for navigation, language switching, the mobile menu and the prepared contact message.
- Added mobile-menu state announcements, Escape-key closing and focus return to the menu toggle.
- Marked the Hero video as decorative and paused it when `prefers-reduced-motion: reduce` is active.
- Improved contrast for copyright text and form placeholders.


## Version 0.7.10 — initialization fix
- Fixed the JavaScript initialization order: the mobile-menu references are now initialized before the default language is applied.
- Restored the execution of the complete site script, including Italian/English switching, mobile navigation and scroll-triggered section reveals.
- Preserved the original scroll-reveal effects and their timing; visitors requesting reduced motion continue to see all content without animated reveals, and the Hero video remains paused.
- No visual design, copy, media, metadata, favicon, responsive layout or contact-form behavior was intentionally changed.
- Tested in Chromium at a mobile viewport: language switching, mobile-menu opening/closing, Escape handling, link navigation, scroll reveals, translation-key coverage and reduced-motion behavior. No JavaScript runtime errors were reported in these checks.
