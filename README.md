# Mally

Mally is a native macOS accounting app for Indian businesses. It does GST, e-Invoice, e-Way Bill, TDS and TCS, payroll, inventory, and full books of accounts, and it runs locally on your Mac with no internet needed for day to day work.

This page is where you download Mally and receive updates.

## Download

[Download the latest version](https://github.com/utkarshrai2811/mally-releases/releases/latest)

Pick the file that matches your Mac:

| File | For your Mac |
|------|--------------|
| `Mally-<version>-arm64.dmg` | Apple Silicon (M1, M2, M3, M4, M5). Almost every Mac sold since late 2020. |
| `Mally-<version>-x64.dmg` | Older Intel Macs only. |

Not sure which one you need? Click the Apple logo at the top left of your screen, choose "About This Mac", and look at the "Chip" line. If it mentions "Apple" (for example "Apple M2"), download the `arm64` file. The Intel file will run on Apple Silicon but it is noticeably slower, so always prefer `arm64` when you have an Apple chip.

## Install

1. Double click the downloaded `.dmg` file. A window opens showing the Mally icon next to your Applications folder.
2. Drag the Mally icon onto the Applications folder in that window.
3. Eject the disk image (Control click it in Finder and choose Eject), then open Mally from Applications or Launchpad.

## First launch: if macOS says "Mally is damaged and can't be opened"

Mally is safe and is not damaged. You see this message because the app is not yet signed with a paid Apple certificate, so macOS blocks apps it cannot verify after they are downloaded from the internet. Here is how to open it, one time only:

1. In the warning dialog, click **Cancel**. Do not click "Move to Bin".
2. Open the **Terminal** app. Quickest way: hold **Command** and press **Space**, type `Terminal`, and press **Return**.
3. Copy the line below, paste it into Terminal, and press **Return**:

   ```bash
   xattr -dr com.apple.quarantine /Applications/Mally.app
   ```

4. Now open Mally normally from Applications. It will open every time after this.

What that command does: macOS adds a hidden "downloaded from the internet" tag to the app, and that tag is what triggers the block. The command removes the tag. You only run it once per install. On older versions of macOS you might instead see "unidentified developer", in which case you can simply Control click the Mally app and choose **Open**.

## Getting started

When Mally opens for the first time you can either set up your own business or explore a ready made demo.

- **Your own company:** click **Create Company**, then enter your business name, GSTIN, home state, and financial year. You are ready to record vouchers right away.
- **Just exploring:** click **Load Sample Company** on the start screen. This builds a fully populated demo business for you (sales and purchase invoices, payroll, ledgers, and reports) so you can try everything without typing in real data. Delete it whenever you like.

Throughout the app, look for the small **?** icons next to fields. They explain anything that is not obvious in plain language, such as Place of Supply, Reverse Charge, or Tax Regime.

## What Mally does

- **GST:** tax invoices, GSTR-1, GSTR-3B, GSTR-2B reconciliation, and input tax credit tracking.
- **e-Invoice:** IRN and a signed QR code through a GSP, with an offline queue for unreliable connections.
- **e-Way Bill:** generation, Part B updates, validity tracking, and expiry reminders.
- **TDS and TCS:** all common sections, Forms 26Q, 24Q, 16, and 16A, and PF ECR export.
- **Payroll:** PF, ESI, Professional Tax, and income tax for both the new and old regimes.
- **Inventory:** FIFO and weighted average costing, multiple godowns, batch and serial tracking, a manufacturing journal, and bill of materials.
- **Accounting:** full double entry books, bill by bill outstanding tracking, bank reconciliation, and financial statements.
- **Tally migration:** import your masters and transactions from a TallyPrime XML export.
- **Multiple users:** Admin, Accountant, Data Entry, Auditor, and Viewer roles.
- **Automatic backups:** scheduled compressed backups with one click restore.
- **Live statutory updates:** tax rate and threshold corrections reach you automatically, with no reinstall needed.
- **Offline first:** all core accounting works without internet. Online features queue and sync when you reconnect.

## Updates

Mally keeps itself current. When a new version is published it downloads in the background and asks you to restart. You can also check any time inside the app under **About and Updates**.

## Requirements

- macOS 12 Monterey or later.
- An Apple Silicon or Intel Mac. Download the matching file from the table above.

## Need help

Open an issue on the **Issues** tab of this page. Describe what you were doing and what happened, and include your Mally version (shown on the **About and Updates** screen).
