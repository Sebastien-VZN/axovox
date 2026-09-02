# Changelog — Axovox

All notable changes to Axovox are documented here.
Full release notes: [GitHub releases](https://github.com/Sebastien-VZN/axovox/releases)

---

## [beta_0.14.4] — 2026-09-03

### Windows — single instance (fix)
- The app could previously be opened multiple times on Windows: clicking a toast notification or relaunching the executable started a new process instead of bringing back the running one (the close button only hides the window to the system tray, so duplicate processes piled up: two tray icons, two live connections, concurrent local database writes)
- Axovox now enforces a single instance: a second launch brings the existing window back to the foreground — even when it was hidden in the tray — and exits instantly
- Clicking a toast notification now restores the running app and opens the relevant page, instead of spawning a duplicate

### Linux — single instance (fix)
- The same duplicate-process issue existed on Debian: the default Flutter Linux template explicitly disabled GtkApplication's native single-instance behavior
- Axovox now uses the native D-Bus single-instance mechanism: a second launch forwards its arguments to the running instance, presents its window and exits — same behavior as Windows, including toast payload routing

### Security — logout data purge
- Logging out now clears in-memory session state before touching the disk: the open conversation's messages, active bots, and the outgoing account's theme and language preferences are wiped — the next account signing in on the same machine inherits nothing from the previous one
- A failure to delete the local cache folder (e.g. a file still locked by the OS on Windows) no longer aborts the rest of the logout chain

### Messenger
- Online/offline indicator now also shown in the user profile sheet; group name added to the group profile sheet
- First-visit panels (no contacts yet / no groups yet) now show the navigation button on mobile

### Maintenance
- Windows notifications: stable AppUserModelId and a dedicated notification GUID, so Axovox and Axomind can coexist on the same machine without registry conflicts
- Uploads rejected because the server storage is full now show a dedicated message instead of a generic error
- Language package updates across the 33 supported languages
- Flutter and Android Gradle upgrades

---

## [beta_0.14.1] — 2026-08-21

- GitHub workflow fixes after the AuroriaLink → Axovox rename
- CI token handling and test fixes

## [beta_0.14.0] — 2026-08-21

Period: May 2026 to August 2026 — 44 commits, 466 files changed.

### New name: Axovox (formerly AuroriaLink)
- Complete rebrand to "Axovox" — shorter, memorable, aligned with the Axomind ecosystem
- Same product, same codebase, new identity across the app, CI/CD, GitHub repository and documentation

### Native spell check — migrated to OS-level checking
- Replaced the old in-app custom spell checker (`GstSpellCheck`, 363 lines) with our `native_spell_checker` fork, published on GitHub
- Uses the OS-native spell checker directly: WinRT `ISpellChecker2` on Windows, `libhunspell-1.7` on Linux, Flutter's `DefaultSpellCheckService` on Android
- Zero bundled dictionaries — the OS provides everything
- `SpellCheckTextFormField` as a drop-in replacement for `TextFormField`
- 100% offline, no cloud APIs

### 33 languages with native flags
- Full UI translation across 33 languages, matching flag icons for every language

### 27 themes with light and dark variants
- Each theme ships with light and dark variants
- Colors extracted to the `quodexus_color` shared package (7,139 lines removed from the app, now maintained as a standalone dependency)
- Background animations: Aurora, particles, cyberpunk and retro terminal effects
- Glassmorphism effects via `BackdropFilter` and `ImageFilter.blur` across the UI

### Quota system (rebuilt)
- Completely rebuilt client-side quota management
- Three subscription plans: free, perso and pro
- Per-plan limits on audio recording duration, file size, simultaneous uploads and more

### Messenger
- Major messenger update with improved stability
- Fixed a random instance crash in the messaging module
- Improved scroll and conversation positioning

### Rich text editor
- TextAreaEditor and TextAreaViewerStatic stability and scroll fixes
- Shared core migration for better maintainability

### Mobile and UX
- Fixed mobile animation performance
- Fixed file picker selection
- Multiple Android build and configuration fixes

### Infrastructure
- **CI/CD pipeline rewritten from scratch**: `validate` job (format check, static analysis, unit tests, integration tests), `android-build`, `linux-build`, `windows-build`, `release` job with SHA256 checksums published to both Forgejo and GitHub
- Flutter 3.47.1 (Dart 3.13.1) pinned across all jobs
- Flutter, Dart SDK and Android Gradle Plugin upgraded to latest stable
- Shared core migrated to shared package architecture
- 593 tests across 53 files (core: 193, models: 55, network: 62, security: 24, integration: 259)

## [beta_0.11.0] — 2026-07-07

### Improvements
- **Android notifications reworked** — rebuilt on the native Android API, no more permission conflicts
- **More stable startup** — user preferences and session data loaded at the right time in the startup cycle, preventing occasional crashes

### Fixes
- Random crash in messaging fixed
- Android build: Gradle and Kotlin updated for the latest Android SDKs
- File viewer: improved handling of media files shared in conversations

### Technical
- Flutter dependencies updated
- CI/CD migrated to a more robust infrastructure

## [beta_0.10.5] — 2026-05-26

- Stability fixes and internal adjustments
- Project dependency updates

## [beta_0.10.4] — 2026-05-13

### Messaging
- Major update: better performance, fix for a random crash, improved display on low-resolution phones

### Security
- Better session handling: cleaner logout

### Translations
- French and English texts updated and extended

## [beta_0.10.3] — 2026-05-13

- First rollout of the major messenger update — performance, stability and low-resolution display (stabilized in beta_0.10.4)

## [beta_0.10.1] — 2026-05-10

### Major update
- **Extended permission management for groups** — read-only and write-access participants; only the group creator manages bots and full permissions
- **Improved messenger** — smoother interface on long conversations, better scroll handling, improved automatic URL detection, automatic conversion of long messages to Markdown files
- **Overall performance** — rendering optimization, better memory management during uploads and page transitions, faster and more stable startup
- **Enhanced spell checker** — more comprehensive French/English dictionaries, better elision and compound-word detection, auto-ignores URLs/emails/mentions/hashtags
- **Stability** — numerous connection/disconnection fixes, better resilience on connection loss
- **Miscellaneous** — improved media/file managers, more reliable bot integration, strengthened real-time sync

## [beta_0.10.0] — 2026-05-10

- Global code migration from the Axomind codebase to the AuroriaLink repository
- Documentation, lint and internal fixes

## [beta_0.9.0] — 2026-03-17

### Integrated spell checker
- New local spell checker built directly into the messenger (French + English)
- Smart Check: French elisions, compound words, automatic filtering of URLs, emails, mentions and hashtags
- Levenshtein-based suggestions with caching; native keyboard spell checker on mobile

### Redesigned messaging
- Major messaging refactoring: smoother interface and centralized logic
- Fixed scroll behavior and conversation position
- Improved animations and overall UX design

### Stability & performance
- Async management overhaul: more robust UI with fewer freezes
- Faster and more reliable app startup

## [beta_0.8.4] — 2026-03-03

- Messages now kept for 6 months (instead of 15 days); unpinned files kept for 1 month
- Conversation lifetime saved correctly (a duration change sometimes only took effect after a restore)
- Minor visual improvements in the chat; internal Android components updated; several minor bugs fixed

## [beta_0.8.3] — 2026-02-10

- WebSocket configuration adjustment to prevent rare service interruptions

## [beta_0.8.2] — 2026-02-03

- Unified audio system (`GstAudio`) centralizing playback and user volume handling
- Notification sound preview (`MiniPlayerWidget`) directly from settings
- `notification_locale` refactored onto the new `GstAudio` implementation
- Stricter JSON parsing with enriched debug logs
- UI adjustments: button centering and harmonized border thickness

## [beta_0.8.1] — 2026-01-29

- UX fixes in messaging, particularly conversation scrolling

## [beta_0.8.0] — 2026-01-27

- Full bot API integration — bots send messages directly into conversations (`GstDataBots`)
- Integrated search engine for messages and documents
- User blocking (local list synchronized with the server)
- Theme system harmonized: 16 themes (Aurora, Axomind, Forest…) in light and dark modes
- Visual indicators for new messages in threads; mobile ergonomics fixes (audio player, Android navigation)
- Real-time WebSocket updates improved for bots and statuses; Axomind / AuroriaLink module separation clarified

## [beta_0.7.2] — 2026-01-20

- Minor UX fix

## [beta_0.7.1] — 2026-01-19

- 5 new themes: Biohazard, Dracula, Nebula, Retro Term 70 Red, Synthwave (light + dark variants)
- Fixed real-time bot updates via WebSocket; improved bot state and assignment management
- Focus group form, bot management page and date formatting fixes
- Server-side: exchange token security fix, stronger authentication validation

## [beta_0.7.0] — 2026-01-17

- Bot API framework: encrypted token authentication, dedicated message-sending API, management interface in the dashboard, visual distinction between bots and humans
- Extended encryption chains

## [beta_0.6.0] — 2025-12-31

- Visual marker (green separator line) before unread messages, respecting message collapse groups
- Smart unread counters (incremental, reset after 10s or on window focus)
- Desktop integration: systray notification icon and taskbar count badge
- Optimized WebSocket updates without redrawing the whole conversation list

## [alpha_0.5.5] — 2025-12-30

- Audio module: playback stability fixes, large-file memory management, Debian 13 support

## [alpha_0.5.4] — 2025-12-19

- Copy feature in messaging

## [alpha_0.5.3] — 2025-12-19

- Fix on URL detection

## [alpha_0.5.2] — 2025-12-18

- Desktop system tray (Windows) with notification icon, asset compression, messenger technical redesign (mixins, form management)

## [alpha_0.5.1] — 2025-12-11

- 21 themes (light + dark), 8 chat backgrounds, customizable send shortcut (Enter / Ctrl+Enter), modernized interface

## [alpha_0.5.0] — 2025-12-03

- First 0.5.x rollout — theme system release (detailed notes published with alpha_0.5.1)

## [alpha_0.4.0] — 2025-12-03

- Major structural overhaul: refactored navigation engine + mobile bottom bar, server-side antivirus scanning and file integrity control, new local database for near-instant conversation loading, unified icon set, memory optimizations

## [alpha_0.3.0] — 2025-11-23

- Interface refinement (borders, contrasts, hover states), smart URL detection in the editor, new notification sounds + mute option, WebSocket reliability, dashboard pagination fix

## [alpha_0.2.0] — 2025-11-14

- Centralized email aggregator, externalized server credentials, security and UX fixes — database reset (accounts recreated)

## [alpha_0.1.1] — 2025-11-11

- Safer file upload with automatic validation, desktop minimum window size, instant login after signup, numerous bug fixes

## [alpha_0.1.0] — 2025-11-04

- Stabilization: persistent PDO connections, PostgreSQL index optimization, 3-tier file cache (APCu + ramdisk + Redis), decryption CPU load reduced by 80%, WebSocket heartbeat, multi-device session closure

## [alpha_0.0.6] — 2025-10-30

- Message reactions + UX fixes

## [alpha_0.0.5] — 2025-10-28

- Message lifetime option (24h / 3 months), WebSocket optimization

## [alpha_0.0.4] — 2025-10-24

- WebSocket fix and sync improvement, return-key fix, push notifications

## [alpha_0.0.3] — 2025-10-21

- Stability and reference-loss fixes, visual user guide, file management and resource optimizations

## [alpha_0.0.2] — 2025-10-14

- Message counting, interface opening and group management fixes

## [alpha_0.0.1] — 2025-10-13

- First public alpha build — translation added
