# macos-eset-context-menu
Unofficial Finder context menu (Quick Action) to scan files with ESET Endpoint Security / Endpoint Antivirus / Cyber Security for macOS.

## Prerequisites
- MacOS
- One of the following ESET products:
  - ESET Endpoint Security
  - ESET Endpoint Antivirus
  - ESET Cyber Security

## Install
1. Download the workflow you prefer and unzip it.
   - `EsetScan.workflow`: Shows the scan result in Notification Center.
   - `EsetScanTerm.workflow`: Opens Terminal.app and shows the scan result.
2. Double-click the downloaded `.workflow` file, then click **Install**.
3. In Finder, select files or folders, right-click, and choose **Quick Actions** → **EsetScan** (or **EsetScanTerm**).

If macOS blocks the workflow, run the following command in Terminal and try again:

```zsh
xattr -dr com.apple.quarantine ~/Downloads/EsetScan*.workflow
```

## Uninstall
Delete the workflow from `~/Library/Services`.

## Disclaimer
This is an unofficial tool and is not affiliated with ESET or Anthropic. Use at your own risk.

## Credits
- Design: Y.H.
- Implementation: Written with Anthropic's Claude (Opus 5.5)

## License
MIT
