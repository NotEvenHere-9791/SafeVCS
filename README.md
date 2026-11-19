<div align="center">
  
# SafeVCS Studio


### Intelligent Version Control. Automatic Protection. Complete Peace of Mind.

**SafeVCS Studio** is an offline-first version control and workspace management solution designed to safeguard development projects through automated snapshots, reliable file synchronization, and effortless version recovery.

</div>

---

## Overview

**SafeVCS Studio** brings simplicity and reliability to project version management.

Designed for developers who want dependable version tracking without the complexity of traditional Git workflows, SafeVCS Studio provides an intuitive desktop experience backed by intelligent background automation.

With automatic workspace protection, isolated version history, and one-command recovery, your project remains protected against accidental modifications, unexpected deletions, and system interruptions.

Everything operates locally, keeping your projects and version history under your control.

---

## Key Features

### Reliable Data Protection
- Atomic file operations designed to minimize the risk of data corruption.
- Power-interruption-conscious save mechanisms.
- Reliable background synchronization.
- Automatic workspace protection.

### Intelligent Auto-Save
- Background monitoring of project changes.
- Debounced automatic snapshots.
- Optimized synchronization to reduce unnecessary file operations.
- Manual synchronization whenever required.

### Complete Workspace Preservation
- Comprehensive project file and folder preservation.
- Support for source code, scripts, binaries, assets, and configuration files.
- Preservation of hidden files and nested directories.
- Independent version snapshots.

### Isolated Version Management
- Automatically locks previous versions after committing.
- Maintains a dedicated active working version.
- Preserves historical project states.
- Helps prevent unintended modifications to committed versions.

### One-Command Version Recovery
- Restore previous project versions.
- Recover from accidental file modifications or deletions.
- Return to a known working state.
- Simplified rollback workflow.

### Modern Desktop Experience
- Professional borderless dark interface.
- Integrated file manager and dashboard.
- Hierarchical project navigation.
- Built-in file viewing and text editing.
- Adaptive interface font scaling.
- Dedicated application settings.

### Global Command-Line Integration
- Convenient `svcs` terminal commands.
- Integrated with Windows system PATH.
- Compatible with common development terminals, including PowerShell and VS Code terminals.

---

## Installation

Getting started with SafeVCS Studio is simple.

1. Visit the [Latest Releases](../../releases/latest) page.
2. Download `SafeVCS-Setup.exe`.
3. Run the installer and follow the installation wizard.
4. Open your development project in PowerShell or your preferred terminal.
5. Initialize SafeVCS.

```powershell
svcs init
```

Your project is now protected by SafeVCS Studio.

---

## ⌨️ Command-Line Reference

SafeVCS Studio provides a straightforward command-line interface for managing your project versions.

### 1. Initialize a Project

```powershell
svcs init
```

Initializes SafeVCS for the current project.

**What it does:**
- Creates and initializes the project's version vault.
- Captures the current workspace.
- Configures supported editor auto-save settings.
- Starts the background synchronization service.

### 2. Create a New Version

```powershell
svcs push [version_name]
```

Creates a new version of your current project.

**What it does:**
- Synchronizes the latest workspace changes.
- Locks the previous version against modifications.
- Creates a new active working version.
- Supports custom version names or automatic numbering.

**Examples:**

```powershell
# Create a custom version
svcs push v1

# Automatically generate the next version
svcs push
```

### 3. Restore a Previous Version

```powershell
svcs rollback [target_version]
```

Restores your project to a previously saved version.

**What it does:**
- Preserves the current working state as a separate version.
- Restores the selected historical snapshot.
- Sets the restored version as the active working version.

**Examples:**

```powershell
# Restore a specific version
svcs rollback v0_initial

# Restore the previous version
svcs rollback
```

### 4. Synchronize Project Files

```powershell
svcs sync
```

Or:

```powershell
svcs save
```

Immediately synchronizes the current workspace with its active version.

Useful when you want to manually save your progress without waiting for automatic synchronization.

### 5. View Project Status

```powershell
svcs status
```

Displays an overview of your SafeVCS project.

**Information includes:**
- Project vault location.
- Currently active version.
- Background synchronization status.
- Last synchronization timestamp.
- Available project versions.
- Version access modes and file statistics.

### 6. Launch the Desktop Application

```powershell
svcs app
```

Alternative commands:

```powershell
svcs gui
svcs fm
```

Launches the SafeVCS Studio desktop interface.

**Available functionality:**
- Project dashboard.
- Integrated file manager.
- Version navigation.
- Built-in file viewer and editor.
- Application settings.
- Interface customization.

### 7. Register Command-Line Integration

```powershell
svcs register
```

Or:

```powershell
svcs install-cli
```

Re-registers the SafeVCS command-line executable with the Windows environment to restore global terminal access.

---

## Desktop Application

SafeVCS Studio includes a dedicated graphical interface designed to make project management intuitive and efficient.

Key interface capabilities include:

- **Studio Dashboard:** Access project information and version management features.
- **File Explorer:** Browse project directories and navigate files.
- **File Viewer:** Inspect project files directly within the application.
- **Text Editor:** Open and edit supported text-based files.
- **Version Management:** View and manage historical project versions.
- **Professional Settings:** Customize application preferences and interface appearance.

---

## Privacy & Offline Operation

SafeVCS Studio is designed around local-first project management.

- No cloud synchronization required.
- No mandatory online account.
- Project version management operates locally.
- Your project files remain under your control.
- No external repository hosting is required.

Your development workflow stays local, private, and independent.

---

## Building from Source

For developers interested in building the application distribution package:

**Requirements:**
- Python environment.
- Required project build dependencies.
- Inno Setup Compiler.
- Application branding assets.

Execute the provided build script:

```powershell
python build_safevcs.py
```

After successful compilation, open the installer configuration in Inno Setup Compiler and compile it using `F9`.

The resulting installer is distributed as:

```text
SafeVCS-Setup.exe
```

---

## Command Quick Reference

| Command | Description |
|---|---|
| `svcs init` | Initialize a project |
| `svcs push` | Create a new version |
| `svcs push <name>` | Create a named version |
| `svcs rollback` | Restore the previous version |
| `svcs rollback <name>` | Restore a specific version |
| `svcs sync` | Synchronize immediately |
| `svcs save` | Synchronize immediately |
| `svcs status` | Display project status |
| `svcs app` | Launch desktop application |
| `svcs gui` | Launch desktop application |
| `svcs fm` | Launch file manager |
| `svcs register` | Register CLI integration |
| `svcs install-cli` | Register CLI integration |

---

## License

**Proprietary Software**

Copyright © 2026 NotEvenHere-9791. All Rights Reserved.

SafeVCS Studio is proprietary and confidential software.

Unauthorized copying, redistribution, modification, reverse engineering, or commercial exploitation of this software or its compiled binaries is prohibited, except as expressly permitted by the applicable license.

For complete licensing information, refer to [LICENSE.txt].

---

<div align="center">

### SafeVCS Studio

**Protect Your Work. Preserve Your Progress. Stay in Control.**

*Reliable version management, built for developers.*

</div>
