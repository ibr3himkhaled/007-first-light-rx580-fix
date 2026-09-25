---

## ❤️ Support My Work

Hi, I'm **Ibrahim Khaled**, an independent developer
creating compatibility fixes for modern games on
older AMD graphics cards.

Developing these fixes involves extensive reverse
engineering, shader analysis, debugging, and testing.

If my work has helped you enjoy a game that wouldn't
otherwise run on your hardware, please consider
supporting my future projects.

### ☕ Support Development

[![GitHub Sponsors](https://img.shields.io/badge/GitHub-Sponsor-EA4AAA?style=for-the-badge&logo=githubsponsors&logoColor=white)](https://github.com/sponsors/ibr3himkhaled)

[![Ko-fi](https://img.shields.io/badge/Ko--fi-Support_Me-FF5E5B?style=for-the-badge&logo=kofi&logoColor=white)](https://ko-fi.com/ibr3himkhaled)

[![Buy Me a Coffee](https://img.shields.io/badge/Buy_Me_a_Coffee-Support-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black)](https://buymeacoffee.com/ibr3himkhap)

[![PayPal](https://img.shields.io/badge/PayPal-Donate-00457C?style=for-the-badge&logo=paypal&logoColor=white)](https://paypal.me/IbrahimKhaled011)

### 💙 Every Contribution Matters

All donations are completely optional.

My compatibility fixes remain **free and publicly
available**. Your support helps me continue researching,
developing, and improving compatibility solutions
for older GPUs.

Thank you for supporting independent development!

**— Ibrahim Khaled**

---

<div align="center">

# 007 First Light
## AMD Radeon RX 580 Compatibility Fix

**A community-developed DirectX 12 compatibility solution for running 007 First Light on AMD Polaris GPUs.**

![GPU](https://img.shields.io/badge/GPU-AMD_RX_580-ED1C24?style=for-the-badge&logo=amd&logoColor=white)
![API](https://img.shields.io/badge/API-DirectX_12_%2F_Vulkan-0078D6?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D4?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Working-28A745?style=for-the-badge)

**Developed and tested on the AMD Radeon RX 580 8GB.**

[Download Latest Release](../../releases/latest) ·
[Report an Issue](../../issues) ·
[View All Releases](../../releases)

</div>

---

## Overview

This project provides a custom compatibility fix that enables **007 First Light** to run on the AMD Radeon RX 580.

The fix addresses DirectX 12 compatibility limitations, shader model requirements, and graphics pipeline issues that prevent the game from running correctly on older AMD Polaris hardware.

The solution was developed through extensive experimentation with DirectX 12, Vulkan, VKD3D-Proton, custom compatibility components, and GPU feature reporting.

After multiple development iterations, I successfully developed a working Windows compatibility fix for the RX 580.

**The game can now launch and enter gameplay on the tested hardware.**

---

## Features

- Enables 007 First Light to run on the AMD RX 580.
- Addresses DirectX 12 compatibility limitations.
- Includes custom D3D12 compatibility components.
- Uses Vulkan translation to improve compatibility with Polaris GPUs.
- Implements GPU feature reporting workarounds.
- Addresses shader model compatibility problems.
- Provides separate compatibility packages for supported game versions.
- Includes improvements developed through extensive testing and debugging.

---

## Supported Game Versions

The project provides separate compatibility fixes for the following versions:

| Game Version | Fix Available |
|:---|:---:|
| 1.1.0 | Yes |
| 1.1.1 | Yes |
| Other versions | Not Yet |

> [!IMPORTANT]
> Download the compatibility package that matches your installed game version.
>
> The executable modifications differ between supported versions. Do not mix files from different release packages.

---

## Technical Background

The AMD Radeon RX 580 is based on the Polaris architecture.

Running 007 First Light on this GPU presents several compatibility challenges involving modern DirectX 12 features, shader model requirements, and graphics pipeline behavior.

The development process involved:

- DirectX 12 compatibility investigation.
- GPU feature-level and shader-model analysis.
- VKD3D-Proton experimentation.
- Vulkan graphics pipeline debugging.
- Custom D3D12 compatibility components.
- DXGI compatibility investigation.
- AMD Polaris driver debugging.
- Shader compilation analysis.
- Windows and Linux compatibility experiments.

### Compatibility Architecture

The Windows compatibility solution uses custom DirectX 12 components and a Vulkan translation path to address compatibility limitations on the RX 580.

The development process also involved experimenting with GPU feature reporting and the interaction between the game, DirectX 12, and AMD's graphics drivers.

### Windows and Linux Development

The project involved compatibility experiments on both Windows and Linux.

Linux testing with Proton and VKD3D-Proton provided additional information about the game's graphics requirements and Polaris compatibility.

These findings helped guide the development of the Windows fix.

The Windows and Linux implementations are not interchangeable and require platform-specific components.

---

## GPU Compatibility

The primary development and testing target is the **AMD Radeon RX 580 8GB**.

| GPU | Compatibility |
|:---|:---|
| AMD Radeon RX 580 8GB | Successfully tested |
| AMD Radeon RX 570 | Community testing welcome |
| AMD Radeon RX 480 | Community testing welcome |
| AMD Radeon RX 470 | Community testing welcome |
| Other AMD Polaris GPUs | Not fully verified |
| AMD Vega / RDNA | Not verified |
| NVIDIA GPUs | Not verified |
| Intel GPUs | Not verified |

> [!NOTE]
> Compatibility may vary depending on your GPU model, driver version, operating system, and installed game version.

---

## Tested Hardware

The compatibility fix was developed and tested using the following configuration:

| Component | Specification |
|:---|:---|
| GPU | AMD Radeon RX 580 8GB |
| CPU | Intel Core i5-12400F |
| RAM | 16 GB |
| Operating System | Windows 11 |
| Graphics API | DirectX 12 / Vulkan compatibility layer |

---

## Installation

### Step 1 — Download

Visit the official [Releases](../../releases) page.

Download the compatibility package that matches your installed game version.

### Step 2 — Locate Your Game Directory

Open your 007 First Light installation directory.

Locate the folder containing the game's executable and DirectX 12 components.

### Step 3 — Back Up Existing Files

Before installing the fix, back up any existing files that will be replaced.

This is especially important if you have previously installed another compatibility fix.

### Step 4 — Install the Fix

Extract the downloaded package.

Copy its contents into the appropriate game directory, preserving the folder structure provided in the release archive.

Follow any version-specific instructions included with your downloaded package.

> [!WARNING]
> Do not combine components from different game-version packages.
>
> Always use the executable and DLL files supplied together in the same release.

### Step 5 — Launch the Game

Launch the game normally after installing the compatibility package.

---

## First Launch and Shader Compilation

> [!IMPORTANT]
> The first launch may involve extensive shader compilation.

You may experience significant stuttering or temporarily reduced performance while shaders are being compiled.

Depending on your system and shader cache state, subsequent launches may be smoother.

Allow shader compilation to complete before evaluating performance.

Avoid repeatedly terminating the game during its initial compilation process unless it has genuinely crashed or stopped responding for an extended period.

---

## Known Limitations

- The RX 580 8GB is the primary tested GPU.
- Other Polaris models may require additional testing.
- Compatibility depends on the installed game version.
- Different AMD driver versions may produce different results.
- Initial shader compilation may cause significant stuttering.
- Performance depends on graphics settings and system configuration.
- Future game updates may require updated compatibility components.

---

## Development Status

**Status: Working**

The Windows compatibility fix has been successfully developed and tested on the AMD Radeon RX 580 8GB.

Separate compatibility packages have been developed for game versions 1.1.0 and 1.1.1.

Future updates may include additional compatibility improvements, performance optimizations, and fixes based on community feedback.

---

## Bug Reports

If you encounter crashes, startup failures, graphical issues, or other compatibility problems, please open a [GitHub Issue](../../issues).

Include the following information:

1. GPU model and VRAM.
2. AMD driver version.
3. Windows version.
4. Game version.
5. Compatibility fix version.
6. Description of the problem.
7. Steps to reproduce the issue.
8. Relevant screenshots or logs.

Please check existing issues before submitting a new report.

---

## Disclaimer

This is an independent, community-developed compatibility project.

It is not affiliated with, endorsed by, or officially supported by IO Interactive, AMD, or the VKD3D-Proton development team.

007 First Light and all related trademarks belong to their respective owners.

This project does not include the game itself. A legitimate copy of the game is required.

---

<div align="center">

### Developed by Ibrahim Khaled

**Bringing modern games to AMD Polaris hardware.**

[GitHub Profile](https://github.com/ibr3himkhaled)

If this project helped you, consider giving it a ⭐!

</div>
