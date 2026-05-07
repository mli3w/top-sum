# Changelog

All notable changes to **Top Sum** are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the project loosely adheres to semantic versioning.

---

## [v12] — 2026-05-07

### Added
- **NDP-style RSAF fighter flypast** (day-only ambience): 5 jets in arrow formation streak across the bay every ~35–65s with fading white contrails.
- **Star insignia** (★) above the title logo with twinkle + gentle vertical float.
- **Cinematic warm radial bloom** behind the whole title logo.
- **Title intro sequence** (~1.6s, one-shot on first render): wings sweep outward, TOP SUM settles, star drops with a subtle overshoot, subtitle rises last.
- **Ambient title loops**: slow breathing gold pulse on the type; star twinkle + float.
- `@media (prefers-reduced-motion: reduce)` disables all title animations.
- **Sunset unlock celebration** at 1000 pts now includes a full-screen sun-flare bloom, slow-rotating golden sun-rays behind the card, a pulsing halo ring behind the 🌅 icon, and ~46 falling golden sparkle particles in two bursts.
- **`body.sunset-pending` state** glows the in-game ☀ time icon and the title-screen 🌅 Sunset radio until the player engages sunset for the first time (then auto-clears).
- `README.md`, `LICENSE` (MIT), and this `CHANGELOG.md` added to the repo.

### Changed
- **Title logo redesign** — replaced flanking feathered gold wings with a single centered swept-forward delta wing pair in chrome that forms an inverse triangle framing the type, V tip dropping near the · in the subtitle.
- **TOP SUM** now side-by-side same-sized italic gold metallic (was stacked, with SUM in blue).
- Brighter, more inviting gold gradient on the type with a warm amber halo replacing the prior dark vignette.
- Subtitle: letter-spacing tightened ~14%, colour brightened, opacity 0.95 → 1.
- **Open Graph / Twitter card** meta tags now use absolute URLs anchored to `https://mli3w.github.io/top-sum/` with a working `og:image` (previously pointed at a non-existent `share-card.png`).
- `shareScore()` always shares the canonical play URL — never a local `file://` path or query-string variant.

### Fixed
- **Pause overlay buttons** (Resume / Restart / End Flight / Back to Menu) were unclickable on desktop. The overlay sat inside `#hud` (`pointer-events: none`) without re-enabling pointer events on itself.

---

## [v11] — earlier

Path re-route, gate colour scheme, ambient world systems (Chinook + flag, fireworks, MBS Spectra), Sunset Mode unlock at 1000 pts with celebration, single ⏸ pause overlay, first-time onboarding, mobile control tip, Tiny mode arrow assist.

See the comment block at the top of [`index.html`](index.html) for the full v11 / v10 / earlier change history.
