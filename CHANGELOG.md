## 2.7.3 (2026-10-10)

- Add Create required folders automatically under Settings > Paths & Directories for use after initial setup.
- Fill empty optional folder fields while preserving configured paths; use the normal Save action to persist changes.

## 2.7.2 (working preview)

- Add an enabled-by-default Create required folders automatically checkbox to first-start setup.
- Create optional livery/ghost backup, ghost catalogue and author notes folders under TDUSC Companion Data beside the executable, then save their Settings paths.
- Preserve configured paths and existing files; report creation failures without closing setup.

## 2.7.1 (2026-10-10)

- Rename the application to TDUSC Companion, with TDUSC Companion - User Data Suite in the main window title and documentation headings.
- Use TDUSC_Companion for application source and executable filenames.

## 2.7.0 (2026-10-10)

- Native Ghost Catalogue with sharing, original recovery and automatic retention of changed recordings.
- Persistent, optional plain-text Author Notes for ghosts and liveries, limited to 1000 characters.
- Independent viewer and ghost defaults, configurable notes storage and unsaved Settings prompts.
- Community tab, matching-race catalogue filtering and aligned adjustable Ghosts panes.
- Correct cross-drive catalogue paths and first-time note storage; show received livery notes beside previews.

## 2.6.3 (working preview)

- Show read-only Author Notes beside the preview when choosing a shared livery, including downloaded previews.

## 2.6.2 (working preview)

- Add an Author notes folder picker to Settings for livery and ghost note storage.
- Require an explicit external notes folder; include it in persistence and unsaved change detection.
- Do not migrate previous preview notes.

## 2.6.1 (working preview)

- Create note storage directories before saving livery or ghost Author Notes, including imported livery notes.

## 2.6.0 (working preview)

- Add persistent Author Notes to liveries through Actions and the context menu.
- Reuse the share note editor with independent package omission and local note retention options.
- Display received notes before replacing a livery and retain them with the imported design; enforce the same plain-text 1000-character limit.

## 2.5.0 (working preview)

- Add persistent per-recording Author Notes for own ghosts, available through Actions and the context menu.
- Add a share editor with a 1000-character counter and Don't share my note option.
- Import plain-text author notes separately from personal catalogue notes; validate the limit on save, export and import.

## 2.4.9 (working preview)

- Default missing ghost driver names to unknown, including legacy ghost-filename placeholders.

## 2.4.8 (working preview)

- Always hide Navigation, Crown Jewel, Unknown and Unreadable ghosts from both trees; remove their filter checkbox.
- Add Show matching race only as the saved Ghosts default filter in Settings.

## 2.4.7 (working preview)

- Automatically detect valid changed recordings during active catalogue sessions, polling every three seconds.
- Require repeated matching content checks, archive the previous original in the catalogue and back up the new recording before completing the session.
- Replace the Keep New Ghost button with automatic handling and a completion notice.

## 2.4.6 (working preview)

- Add Keep New Ghost to retain a changed game recording and complete its catalogue session.
- Validate and back up the kept recording before clearing the session; preserve previous original backups.

## 2.4.5 (working preview)

- Group default filters and sort order in separate Livery Viewer and Ghosts Settings sections.
- Persist independent Ghosts defaults and include them in the unsaved Settings prompt.

## 2.4.4 (working preview)

- Ask whether to save or discard unsaved Settings changes when leaving the tab.
- Apply the initial 50/50 Ghosts split after native resize handling, while retaining manual adjustment.

## 2.4.3 (working preview)

- Align both Ghosts trees and start at 50/50, preserving the adjustable splitter ratio during window resizing.
- Show race, car, replay time and filename below either selected ghost, with full text in a tooltip.

## 2.4.2 (working preview)

- Add Restore My Ghost to the My Ghosts context menu, enabled for races with an active catalogue session.

## 2.4.1 (working preview)

- Accept ghost catalogue folders on a different drive from GAMEDATA.
- Preserve containment checks for GAMEDATA itself and its subfolders, including Windows case differences.

## 2.4.0 (working preview)

- Added Community tab with Markdown categories and clickable website links.
- Added editable community.md with the initial community project list.

## 2.3.0 (working preview)

- Optional in-game alias in shared livery and ghost metadata.
- Show received author aliases and adopt them during ghost catalogue imports.

## 2.2.0 (working preview)

- Added a Ghost Catalogue tree beside My Ghosts, with race grouping and matching-race filtering.
- Added individual and multi-file imports, including collection ZIPs with multiple recordings per race, SHA-256 duplicate detection and import reports.
- Added driver names and notes for catalogue recordings.
- Added Use Ghost, Restore My Ghost and Restore All My Ghosts with durable sessions and verified original snapshots.
- Preserve recordings changed by the game before switching or restoring catalogue ghosts.
- Added catalogue and recovery instructions to the user guide and built-in Howto.

# Changelog

## 2.0.3 — Working build, 2026-10-05

- Use the exact in-game instruction: Apply Livery for c 30 000.


## 2.0.2 — Working build, 2026-10-05

- Rename the sharing guide to howto_share_a_livery.md and format it as Markdown.
- Render headings, bold text, inline code and lists in the Howto tab.


## 2.0.1 — 2026-10-05

- Prefill shared ZIP filenames with the vehicle name and livery timestamp.
- Prefill editor output filenames from the input, with the appropriate JSON suffix.
- Show the associated thumbnail for livery groups and non-image files.
- Remove the Native Preview suffix from the window title.
- Limit future runtime packages to end-user files and license notices.

## 2.0.0 — 2026-10-05 (native preview)

- Adopted semantic versioning and versioned application/build/package filenames.
- Replaced the Python application with the native C++17/wxWidgets port.
- Preserved livery editing, backups, share/replace, telemetry and settings.
- Updated viewer layout and split the telemetry IPv4 address into four fields.
- Added CMake build instructions, bundled SQLite/JSON sources and native packaging.
- Removed the Python application, installation guide and Python build scripts from the current branch.

## 1.01 — 2026-10-04

- Preserved expanded viewer groups, selection, and scroll position when returning from another tab or refreshing.
- Replaced viewer sorting and expansion controls with three toggle buttons.
- Included the matching livery thumbnail as preview.png in shared ZIPs.
- Added a display-only ZIP preview to Replace Livery; only LiveryData is imported.
- Moved Open Source to the bottom-right of the source dialog.

## 1.0 — 2026-10-03

- Added a custom sports car icon for application windows and the executable.

- Added configurable file manager executable and arguments, with Windows and Linux defaults.

- Added first-launch setup to select and save the TDUSC UserSettings folder.

- Added a viewer context menu for editing, backing up, deleting, sharing, replacing, and locating files in Explorer.
- Added permanent deletion with a confirmation that can be disabled in Settings.
- Added readable timestamps alongside original filenames in the viewer.
- Added **Share Livery** to export a LiveryData file as a ZIP archive.
- Added **Replace Livery** to import a local LiveryData file, shared ZIP, or direct HTTP/HTTPS link, with validation and a mandatory backup.
- Added JSON loading through **Open File** in the Livery Editor.
- Added telemetry save choices: overwrite, back up and overwrite, or cancel, with an option to disable the prompt.
- Added an in-app **Howto** tab with separate sending and receiving instructions.
- Switched to a shared `settings.ini`, with fallback loading from earlier version-specific settings files.

## 0.06

- Added a Telemetry tab for enabling telemetry, editing connection settings, and backing up `UserSettings.cfg`.

## 0.05

- Added vehicle thumbnails and their viewer filter.
- Changed vehicle group labels to display the vehicle name before its ID.

## 0.04

- Added vehicle-name lookup through the external `carlist.db` database.

## 0.03

- Added backups for individual liveries and all liveries, with a configurable default backup folder.
- Reorganized the main tabs with the Livery Viewer first.

## 0.02

- Provided the livery viewer and binary/JSON editor.
- Supported LiveryData format versions 4 and 5, including multiple sticker lists.
