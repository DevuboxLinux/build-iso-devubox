### 🧩 Why This Workflow Uses a GUI
The Devubox-MX ISO build script (forked and customized from an upstream project)
requires a text-based interactive interface (TUI) during ISO creation.

Because of this, the GitHub Actions workflow launches a lightweight XFCE desktop
and VNC server, allowing developers to connect, run the build script manually,
and test the distro graphically inside the runner environment.

This setup is only for safe, local interaction — no external RDP or remote access
beyond the current GitHub Actions session is used.
