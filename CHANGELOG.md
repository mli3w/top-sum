# Changelog

All notable changes to **Top Sum** are documented here.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and the project loosely adheres to semantic versioning.

---

## [v13] — 2026-05-10

The biggest update since launch. New ZOOOM cinematic boost, Speed Mode for fast players, redesigned title logo, sunset bumps, and an RSAF flypast over Marina Bay.

### Added
- **ZOOOM cinematic boost** — pill-shaped bar fills as you answer correctly (5/7/10 streak by difficulty). Once full, tap or press `Z` to fire a 3/4-of-circuit cinematic lap:
  - Big italic "ZOOOM" word flies across the screen at activation
  - Two F-16 escort jets fade in from the rear, lock onto your flanks, then peel off climbing-and-outward in the final 15% of the lap
  - Each wingmate emits a glowing additive-blend vapor trail (80-sample point cloud)
  - Camera FOV widens from 72° to 92° for a warp-tunnel feel
  - Spinning radial speed-streaks overlay + bright edge vignette
  - Fireworks force-fired across the bay every 0.28–0.50s during the lap (bypasses sunset gating)
  - 3-note rising sting (C5/E5/B5) + low-frequency sawtooth engine swell at activation
  - G-force camera shake on activation
  - Tap mid-question = "ZOOOM ARMED" — auto-fires after the answer settles, never rug-pulls a question
  - Math layer suspended for the lap; base speed × 2.2; gates removed
- **Speed Mode** (50% faster base × flow speed) — title-screen checkbox + in-game `⚡` icon (visible on touch and desktop) + `S` keyboard shortcut. Persists to localStorage. Stacks with Flow multiplier and ZOOOM.
- **NDP-style RSAF fighter flypast** in day mode — 5 jets in arrow formation streak across the bay every ~35–65s with fading white contrails.
- **Star insignia (★)** above the title logo with twinkle + gentle vertical float.
- **Cinematic warm radial bloom** backdrop behind the title logo.
- **Title intro sequence** (~1.6s, one-shot): wings sweep outward, TOP SUM settles, star drops with a subtle overshoot, subtitle rises last.
- **Ambient title loops**: breathing gold pulse on the type; star twinkle + float.
- **Sunset Mode unlock celebration** at 1000 pts now includes a full-screen sun-flare bloom, slow-rotating golden sun-rays behind the card, a pulsing halo ring behind the 🌅 icon, and ~46 falling golden sparkle particles in two bursts.
- **`body.sunset-pending` indicator** — glows the in-game ☀ time icon and the title-screen 🌅 Sunset radio until the player engages sunset for the first time, then auto-clears.
- **Title-screen keyboard hint** now surfaces all six shortcuts (C / M / T / S / Z / ESC).
- `prefers-reduced-motion` disables every new title and ZOOOM animation.
- `README.md`, `LICENSE` (MIT), and this `CHANGELOG.md` added to the repo.

### Changed
- **Title logo redesigned** — single centered swept-forward delta wing pair in chrome forming an inverse triangle that frames the type; V tip drops near the · in the subtitle. TOP SUM now side-by-side same-sized italic gold metallic (was stacked, with SUM in blue). Brighter gradient and warm amber halo replacing the prior dark vignette.
- **Sunset firework palette** doubled — added green / cyan / orange / purple / lime (10 colours total).
- **Sunset firework cadence** tightened from 6–8s to 4–5.5s for a slightly denser sky.
- **Subtitle** letter-spacing tightened ~14%, colour brightened, opacity 0.95 → 1.
- **Open Graph + Twitter card** meta tags now use absolute URLs anchored to `https://mli3w.github.io/top-sum/` with a working `og:image` (234KB PNG — was a 15MB animated GIF that exceeded the 5MB cap on LinkedIn / Slack / WhatsApp, causing share previews to drop to plain links).
- `shareScore()` always shares the canonical play URL — never a local `file://` path or query-string variant.

### Fixed
- **Sunset Mode unlock celebration** "Try it now / Maybe later" buttons were unclickable on desktop. Same root cause as the v12 pause overlay fix — overlay nested inside `#hud` (`pointer-events: none`) without re-enabling pointer events.
- **Wingmate orientation** in earlier ZOOOM iterations had jets facing perpendicular to flight direction; fixed by replacing `lookAt()` with a `Matrix4.makeBasis()` approach that maps the jet model's local +X (nose) onto the path tangent directly.
- **Wingmate roll direction** was reversed (banked opposite of player input); sign flipped so wingmates now bank into the player's turns.

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
