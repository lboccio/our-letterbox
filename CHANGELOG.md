# Changelog — Our Letterbox

All notable changes to this project are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased] — dev branch
Work in progress. Not yet merged to production.

---

## [0.6.0] — 2026-04-05
### Changed
- Dev-only download/copy buttons are now hidden from the live production app (`IS_DEV` flag gates visibility based on hostname)

---

## [0.5.0] — 2026-04-05
### Added
- Audio download button now uses a dropdown menu (▾) with separate Copy and Download options
- Dropdown closes on outside click

---

## [0.4.0] — 2026-04-05
### Added
- Copy to clipboard button for letter text in dev letter actions panel

---

## [0.3.0] — 2026-04-05
### Changed
- Audio download now converts recording to MP3 format using `lamejs` before downloading (previously raw audio)
- Added `lamejs` via CDN

---

## [0.2.0] — 2026-04-05
### Added
- Dev-only download row visible when `IS_DEV` is true (localhost, `.dev` hostname, or `?dev` query param)
- Download button for letter text (plain text export)
- Download button for audio recording

---

## [0.1.0] — 2026-04-01
### Added
- **Edition toggle** — switch between Romantic and Platonic modes; each edition has its own color palette, tone, and copy
- **Platonic edition** (`platonic.html`) — full standalone edition with friendship-appropriate language and styling
- **Reply feature** — recipients can reply to a received letter; reply is threaded back to the original
- **Request a reply toggle** — sender can flag a letter as requesting a reply; recipient sees a banner prompt
- Reply indicator (↩) shown in letter metadata and stamp view when a letter is a reply
- `.gitignore` added for `.vercel`, `.claude/`, `*.backup.html`, `.mcp.json`

---

## [0.0.3] — 2026-03-28
### Changed
- Card box visual polish and font refinements
- Auth flow planning groundwork added to codebase
- Read receipt / rules logic updates

---

## [0.0.2] — 2026-03-27
### Added
- Multi-song embeds — attach more than one song to a letter
- Split sound section UI for cleaner song display
- General UI polish pass

---

## [0.0.1] — 2026-03-27
### Added
- Initial stable version of the letterbox app
- Core features: compose, send, receive, open letters with wax seal animation
- Supabase backend for letter storage and real-time sync
- Vercel deployment configuration (`vercel.json`)
- Romantic edition baseline UI (Playfair Display + Lato typography, gold/ivory palette)
- Audio recording support (voice memos attached to letters)
- Song attachment (single song embed per letter)
- Headspace section (private note visible only to sender after sending)
- Custom BrushPen font embedded as base64

---

*This project uses a `main` / `dev` branch workflow. The `dev` branch holds active work; `main` is the stable production branch deployed to [our-letterbox.vercel.app](https://our-letterbox.vercel.app).*
