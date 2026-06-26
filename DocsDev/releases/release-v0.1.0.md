![v0.1.0](https://github.com/LucasOl1337/CloakBrowser/releases/download/v0.1.0/v0.1.0-card.png)

# v0.1.0 - CloakBrowser baseline (26/06/2026)

Baseline GitHub Release for the writable `origin` repository. The tag already existed; this release records the factual project state without moving the tag or changing runtime code.

## Novidades

- **Stealth Chromium wrapper:** CloakBrowser provides Python and JavaScript APIs that launch a patched Chromium binary while keeping familiar Playwright and Puppeteer-style usage.
- **Drop-in browser APIs:** the repository documents `launch`, `launch_context`, persistent contexts, async Python helpers, and JavaScript launch helpers.

## Melhorias

- **Humanized interactions:** `humanize=True` adds mouse curves, keyboard timing, and scroll behavior for flows that need browser interaction closer to normal user input.
- **Proxy-aware identity:** launch options cover HTTP and SOCKS5 proxies, timezone, locale, GeoIP-assisted configuration, and WebRTC IP controls.

## Correcoes

- **Automation signal hardening:** source-level Chromium patches cover browser fingerprint surfaces such as webdriver, canvas, WebGL, audio, fonts, GPU, screen properties, and automation signals.

## Sistemas

- **Checksum verification:** binary downloads are validated with SHA-256 checksums before use.
- **Package distribution:** the repository includes Python package metadata, JavaScript package support under `js/`, Docker usage, tests, and examples.

---

## Notas tecnicas

Base: existing `v0.1.0` tag in `origin`. This release is a GitHub Release baseline for the fork repository because the upstream `CloakHQ/CloakBrowser` Release is read-only for the current token. Gates for this run: release card generation passed; `python -m pytest -m "not slow"` was attempted and failed in this Windows environment with missing `playwright` plus existing path/platform assertions.
