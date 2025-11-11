[README.md](https://github.com/user-attachments/files/23477613/README.md)
# KlasterApp Build & Release Automation

This folder contains files to automate building and releasing the Windows `.exe` using GitHub Actions.

## Files

- `.github/workflows/build-and-release-windows.yml` — workflow to build and publish EXE automatically
- `main.spec` — PyInstaller build configuration
- `README.md` — this file

## Setup Instructions

1. Copy the `.github` folder and `main.spec` to the root of your project.
2. Commit and push to your `main` branch on GitHub.
3. Go to **Actions** tab in your repo → run the workflow manually or push a tag like `v1.0.0`.
4. After build completes:
   - The EXE will appear in workflow artifacts.
   - If tag was pushed, a new GitHub Release will be created with the EXE attached.

That's it! 🎉
