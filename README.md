# Pwsh-Windows-Admin-Scripts

A collection of PowerShell scripts designed to automate Windows post-installation and routine administration tasks. This repository provides streamlined utilities to configure system settings, optimize performance, manage network protocols, and remove unwanted default applications.

## Included Scripts

* **`ConfigureFeatures.ps1`**: Automates the enabling or disabling of specific Windows features.
* **`ConfigureFirewall.ps1`**: Manages and customizes Windows Firewall rules for improved network security.
* **`ConfigureServices.ps1`**: Configures the startup types and states of various default Windows services.
* **`DisableUnneededNWProtocols.ps1`**: Disables legacy or unnecessary network protocols to reduce system attack surfaces.
* **`SSDOptimizations.ps1`**: Applies specific system optimizations tailored for Solid State Drives (SSDs).
* **`Win10RemoveUWPapps.ps1`**: Removes built-in bloatware and default Universal Windows Platform (UWP) apps from Windows 10/11.

## Prerequisites

* Windows 10 / 11 or Windows Server equivalents.
* Windows PowerShell 5.1 or newer.
* **Administrator privileges** are strictly required to run these scripts, as they modify core OS configurations.

## Usage

1.  Clone the repository to your local machine:
    ```powershell
    git clone [https://github.com/gxjit/Pwsh-Windows-Admin-Scripts.git](https://github.com/gxjit/Pwsh-Windows-Admin-Scripts.git)
    ```
2.  Navigate to the repository directory:
    ```powershell
    cd Pwsh-Windows-Admin-Scripts
    ```
3.  Open an elevated PowerShell prompt (Run as Administrator).
4.  Execute the desired script. *(Note: If your system restricts running downloaded scripts, you may need to temporarily bypass the execution policy)*:
    ```powershell
    Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
    .\Win10RemoveUWPapps.ps1
    ```

## License

This project is open-source and licensed under the [MIT License](LICENSE).
