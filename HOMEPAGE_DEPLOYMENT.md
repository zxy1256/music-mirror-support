# Music Mirror product homepage

## Deploy

The homepage replaces `docs/index.html` in the existing support website. `docs/support.html` and `docs/privacy.html` remain unchanged. There are no dependencies, build commands, JavaScript, external fonts, or external image requests.

1. Review and merge this branch into `main`.
2. If GitHub Pages already serves `main` / `docs`, its next successful deployment will publish the homepage. Otherwise choose Settings → Pages → Deploy from a branch → main → /docs → Save. The expected default address is https://zxy1256.github.io/music-mirror-support/ (not verified as live by this change).
3. Check the published homepage at mobile and desktop widths, follow all three download buttons, and confirm Support and Privacy open correctly. Preserve any existing custom domain or Pages configuration.

Any static host can serve the entire `docs` directory unchanged. Do not upload index.html alone, because the support/privacy links are relative.

## Download verification — October 14, 2026

Verified Apple listing: https://apps.apple.com/us/app/music-mirror/id6762572883
Name: Music Mirror. Developer: Xinyu Zhang. Listed free, for iPhone/iPad; requires iOS/iPadOS 18.5+. Link is used in all three CTAs.

The listing supports playlists, reference demos (YouTube/Files/Photos), written and voice notes, practice timer, audio recording, replay, and user-initiated sharing. Local storage and no-account language follow docs/privacy.html. External content is subject to its provider's privacy practices.

Source checked: zxy1256/music-mirror master (0684667eac86b8f4a655e5799ce59ca72936aed1), root PianoBuddy_PRD.md, DataModels.swift, and MainPracticeViewController.swift. The PRD is planning material, not proof of shipping. Sheet-music photos appear in the PRD/data model but were omitted from marketing because availability in the App Store build was not established. Calendar statistics, practice streaks, video self-recording, automatic feedback, cloud sync and teacher portals are not advertised. The visual is explicitly labeled illustrative, not an app screenshot.

No testimonials, user counts, download totals, acquisition results, signup collection or analytics have been added. Download attribution is not implemented; App Store Connect is required to assess actual installs.

## Validation

Checked HTML structure and section anchors, unique IDs, one H1, all three exact App Store destinations and HTTPS links. Responsive CSS includes a mobile breakpoint, visible keyboard focus, reduced-motion support, and a skip link. Browser visual QA was unavailable in the execution environment; perform the viewport checks above before production release.
