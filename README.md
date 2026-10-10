# TDUSC Companion - User Data Suite 2.7.1

## Getting started

Extract the ZIP into a writable folder and run
`TDUSC_Companion_v2.7.1.exe`. Python is not required. Keep the included
files together. On first launch, select the game user folder containing
`UserSettings.cfg` and `UserOptions.cfg`. Preferences are saved in
`settings.ini` beside the executable.

## Liveries

The Livery Viewer groups files by vehicle and timestamp. Select a file to
preview it. Use filters, sort buttons and expand/collapse to navigate.
Refresh List reloads files after changes made outside the application.

Back up a selected livery or all liveries before editing. Backups include
filtered files and associated images. Select a backup folder in Settings.

Edit Livery opens LiveryData as JSON. The Livery Editor can open binary or
JSON files, save JSON and convert JSON back to binary.

Share Livery creates a ZIP containing LiveryData and an optional preview.
Replace Livery accepts local LiveryData files, shared ZIPs or direct HTTP/HTTPS
links. It backs up the target before replacing its LiveryData. The target
filename is preserved; preview images are never imported. Use a design for
the same vehicle model. Follow the built-in Howto guide for in-game steps.

The right-click menu provides edit, backup, share, replace, delete and open
in file manager actions. Deletion is permanent; create a backup first.

## Telemetry and settings

Close the game before saving telemetry settings. Configure enabled status,
rate, IPv4 address and port in the Telemetry tab. Use the backup button or
choose backup and overwrite when saving. Unrelated config data is preserved.

Settings controls folders, file manager, filters, sorting and confirmation
preferences. Save All Settings stores your choices.

## Included files

- `TDUSC_Companion_v2.7.1.exe`: Windows application.
- `carlist.db`: vehicle names.
- `howto.md`: instructions used by the Howto tab.
- `livery_icon.png`: application icon.
- `README.md`: this guide.
- `THIRD_PARTY.txt`: third-party license notices.

This package is for Windows. Linux has not been tested.

# How to share liveries and ghosts

Choose the sending or receiving instructions for liveries or ghosts. Set your backup destinations in **Settings**.

## Sending a livery

1. Open the **Livery Viewer** in TDUSC Companion.
2. Select the livery you want to share, or one of its files.
3. Click **Share Livery**, or choose **Share Livery** from the right-click menu.
4. Choose where to save the ZIP archive. The suggested filename includes the vehicle name and livery timestamp, for example `Ford_Mustang_GT_20261005123045.zip`. Keep the vehicle name so the recipient can identify the intended vehicle.
5. Send the ZIP archive to the recipient. It contains the LiveryData file and, when available, an optional preview image.

## Receiving a livery

1. Keep an **untouched copy** of the received ZIP or LiveryData file as a backup. You do not need to extract ZIP archives created by **Share Livery**.
2. In the game, create a new livery for the vehicle the shared design is intended for.
3. Place any sticker on the vehicle. This creates a LiveryData file that you can replace with the shared design.
4. Go back and choose **Apply and Save**, then **Save Without Applying**.
5. In your **Livery Collection**, select the default livery, then return to **Workshop > Cosmetic > Livery**.
6. In TDUSC Companion, open the **Livery Viewer** and click **Refresh List**.
7. Select the livery you just created, using the vehicle and timestamp to identify it. You can select its group or one of its files.
8. Click **Replace Livery**, or choose it from the right-click menu. Use **Browse...** to choose a received LiveryData file or ZIP archive, or paste a direct HTTP/HTTPS download link. Click **Open Source** to continue.
9. Confirm the replacement. The program backs up the target livery first, then replaces its LiveryData contents while keeping the target filename. If no default backup folder is set, choose a backup destination. Existing preview images may still show the previous design.
10. Return to the game and open **Livery Collection**. Select the livery you created in step 2 and choose **Edit**, then **Apply & Save > Apply Livery for c 30 000.**
11. The shared design should now appear on your vehicle.

## Important for liveries

The shared livery must contain a **LiveryData file** and must be intended for the recipient's vehicle. **Paint-only changes cannot be shared this way.**

Only the **LiveryData file** needs to be transferred. Always keep backups of both the received file and the file you replace in your `GAMEDATA` folder. The optional ZIP preview is for viewing only and is never imported.

## Sending a ghost

1. Open the **Ghosts** tab and click **Refresh List**.
2. Select the ghost using its race name, vehicle and replay duration. Expand its entry to see the original filename.
3. Click **Share Ghost**, or choose it from the right-click menu.
4. Choose where to save the ZIP. The suggested name contains the race, car and replay duration.
5. Send the ZIP to the recipient. It contains the unchanged original ghost file and **info.txt** with race, vehicle and recording details.

## Receiving a ghost

1. Keep an untouched copy of the received ghost or ZIP. ZIPs created by **Share Ghost** do not need to be extracted.
2. In the game, leave the **race lobby** before replacing the ghost. You do not need to close the game completely.
3. Open **Ghosts** in TDUSC Companion and click **Refresh List**. Select your existing ghost for the same race. The entry or its filename branch can be selected.
4. Click **Replace Ghost**, or choose it from the right-click menu. Browse to a ghost binary file or ZIP, or paste a direct **HTTP/HTTPS download link**.
5. Click **Load Source** to download a link or load a typed path. Browsing loads the file immediately. Review the recording details and, when included, the ZIP's **info.txt**. Click **Use Source** to continue.
6. Confirm the replacement. The program always backs up the original ghost first, then replaces its bytes while keeping your target filename. Set **Default ghost backup folder** in Settings to choose its independent default destination; otherwise the program asks for a ghost backup folder.
7. Return to the race lobby to load the shared ghost. The replay duration may differ from your personal best; replacing a ghost does not necessarily change your saved best time.

## Important for ghosts

Use a ghost for the **same race**. ZIP imports require the original ghost filename to match your selected target. Bare binary files may have arbitrary filenames, so choose the matching race carefully. Ghosts with unreadable contents cannot be shared or imported, but their existing bytes can still be backed up.

Time means **replay duration**, not a verified leaderboard time. ZIP info.txt is descriptive text; it is displayed but never copied into GAMEDATA. Ghost ZIPs do not require a preview image. No METADATA or personal-best data is modified. Keep the original and received backups. To restore an original, select its backup through **Replace Ghost** while outside the race lobby.

### Ghost catalogue

1. In **Settings**, choose a **Ghost catalogue folder** outside GAMEDATA and save the settings.
2. In **Ghosts**, click **Import Ghosts / ZIP**. Select individual ghosts, shared ZIPs or a collection ZIP containing many ghosts. You can select several source files at once. Original ghost filenames must be preserved; ZIPs may contain subfolders and multiple recordings with the same filename. Invalid recordings are reported and identical content is skipped. Import does not replace game files.
3. Your own ghosts appear on the left in **My Ghosts**. Alternatives appear on the right in **Ghost Catalogue**, grouped by race. Select your own ghost to filter matching alternatives, or disable **Show matching race only** to browse everything.
4. Select an alternative and use **Ghost Details** to edit its driver name and notes. The collection filename supplies the initial driver label; it is not proof of the recording's author.
5. Leave the race lobby, select the alternative and click **Use Ghost**. Your existing recording is backed up before the alternative is installed. You must already have your own ghost with the matching filename. Your original remains visible on the left with a catalogue-active marker.
6. You can switch between alternatives without losing the first original. When finished, leave the race lobby and click **Restore My Ghost**, or **Restore All My Ghosts** to restore every affected race.

Active entries and original snapshots are stored in **ghost_sessions** beside the executable, separately for each game user folder. They remain available after a tool restart and do not depend on the catalogue directory being present. Keep this folder when updating or moving the tool; update in the same application directory while a session is active.

If the game writes a new or changed recording while an alternative is active, the tool preserves that file in the session's **changed** folder before switching or restoring. Original snapshots remain available after restoration. Failed restorations remain in the session for retry; a corrupt original backup stops restoration rather than overwriting the game file. The game may remain open throughout; stay outside the race lobby for each swap.

### Optional author alias

In Settings, enter your In-game name and enable Include my alias in shared data.
Save All Settings. Sharing a livery or ghost then includes the alias in
metadata.json; ghost info.txt also shows it. Leave the option disabled to omit
this information. The default is disabled.

Received aliases are displayed when replacing liveries or ghosts. Ghost
catalogue imports use the alias as the driver name, which remains editable.
For collection ZIPs, metadata.json applies to recordings in the same ZIP folder.
Older packages without metadata remain supported. Reimporting an existing
recording does not overwrite manually edited driver names or notes.
Aliases are voluntary, self-reported author labels, not verified account identities.

The Ghosts Tree view includes one combined checkbox for Navigation, Crown Jewel,
Unknown and Unreadable ghosts. Checked shows all four types; unchecked hides them
in both trees. Other races remain visible. This display filter does not exclude
original ghosts from Backup all or active sessions from Restore All My Ghosts.

## Community Projects

The Community tab lists community resources. Select All projects or a category
from the dropdown. Website links open in the default browser.

Edit community.md beside the executable to maintain the list. Each ## heading
becomes a category; ### headings identify individual projects. Use ordinary
Markdown links: [Project name](https://example.com). Links are displayed with
their destination URL visible. The file is loaded at application startup.
Only HTTP/HTTPS links are opened. No embedded HTML or remote images are loaded.
## Automatic New Ghost Detection

While the suite is running, active catalogue sessions are checked every three seconds.
When a changed recording is valid and its content matches on two checks, your previous original is added to the catalogue, the new recording is backed up and remains in GAMEDATA, and the session is completed.
The suite shows a completion notice. Restore My Ghost remains available while the catalogue recording is unchanged.
If import or backup fails, the session remains active and the check is retried. File dates and faster times are not required.

## Author Notes

Select an own ghost and use Author Notes in Actions or its context menu to save a plain-text note of up to 1000 characters. Notes are attached to recording content and stored beside the application, outside GAMEDATA.
Share Ghost opens the note editor before the save dialog. Don't share my note excludes the text from the package. Keep this new note in My Ghosts independently controls whether edits replace the saved local note; it is enabled by default. Cancel leaves saved notes unchanged.
Received Author Notes appear read-only in Ghost Details, separately from editable personal Notes. Older packages without notes remain supported.

## Livery Author Notes

Use Author Notes in Livery Viewer Actions or the context menu to save a note for the selected design. Share Livery opens the same note editor as Share Ghost. Don't share my note excludes the text from the ZIP; Keep this new note in My Liveries controls whether edits replace your saved note.
Received notes are displayed as plain text before replacement and saved with the imported design. Notes are stored outside GAMEDATA beside the application and limited to 1000 characters on save, import and export.

## Author Notes Storage

Choose Author notes folder in Settings before saving notes. Livery notes are stored in its liveries subfolder; ghost notes in ghosts, grouped by game folder. The selected folder must be outside GAMEDATA. Earlier preview note folders are not migrated.


## Download

Get the compiled Windows ZIP from [Releases](https://github.com/mrzworg-dev/TDUSC_Companion/releases/latest). This repository contains documentation and binary releases. Application source is maintained separately in a private repository.
