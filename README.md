# FUD Spyware for the O.M.G Plug/Cable

This repository contains two scripts:

1. **Ducky Script**: Automates the execution of a PowerShell script via simulated keystrokes.
2. **PowerShell Script**: Extracts saved Wi-Fi passwords and screenshots, then uploads them to a remote server.

## Contents

- `ducky-script.txt`: The Ducky Script file.
- `fud.ps1`: PowerShell spyware script.

## Features

- **Wi-Fi Password Extraction**: Retrieves all saved Wi-Fi profiles and their passwords.
- **Screenshot Capture**: Takes periodic screenshots of all screens.
- **Remote Upload**: Uploads extracted data securely to a remote cloud server.
- **Cleanup**: Removes temporary files and clears execution history to maintain discretion.

## Usage

1. **Ducky Script**:
   - Simulates keystrokes to execute the PowerShell script.
   - Downloads `fud.ps1` from a specified URL and runs it.

2. **PowerShell Script**:
   - Defines the `Nextcloud-Upload` function to handle file uploads.
   - Deletes run history from the Windows Registry.
   - Exports Wi-Fi profiles and saves passwords to a text file.
   - Captures screenshots at set intervals.
   - Uploads the collected data to your Nextcloud server.
   - Cleans up by deleting all temporary files and traces.

## Configuration

- **Nextcloud Settings**:
  - Update `$nextcloudUrl` with your Nextcloud server URL.
  - Replace `$sharetoken` with your Nextcloud share token.

- **Directories**:
  - Modify the `$p` variable if you prefer a different working directory.

## Disclaimer

Use this code responsibly and only on systems where you have explicit permission to operate. Unauthorized access or data collection is illegal and unethical.
