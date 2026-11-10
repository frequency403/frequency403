# Hi, I'm Oliver 👋

Software engineer from Germany working in **C#/.NET** and **Rust**. I build CI/CD pipelines and release automation, desktop applications, and software that talks to hardware.

My day job is software for the digitalization of emergency medical services: build and release pipelines, Windows desktop clients, smart card readers and mobile broadband connectivity. In my own time I work on open-source tools around SSH, smart cards and software licensing.

## What I work on

- **CI/CD:** GitLab CI on Windows runners with the PowerShell executor, Jenkins, GitHub Actions with composite actions and reusable workflows
- **Release automation and packaging:** NuGet with pre-release versioning and Central Package Management; tag-driven GitHub releases built from the binaries of the CI run that passed; winget, AUR and NSIS installers
- **Desktop applications:** Avalonia, WPF and WinForms; reactive MVVM with ReactiveUI and DynamicData; moving legacy applications onto the .NET Generic Host
- **Smart cards and secure channels:** PC/SC, ISO 7816-4 APDUs and ATR parsing, PACE and Secure Messaging, German eGK
- **Native interop:** COM interop, Windows Mobile Broadband API (MBN), proprietary serial protocols with binary framing

## Featured projects

### [OpenSSH-GUI](https://github.com/frequency403/OpenSSH-GUI) · C# · Avalonia

Cross-platform desktop app for managing SSH keys, `known_hosts` and `authorized_keys` on Windows, Linux and macOS. Key generation, OpenSSH ⇄ PuTTY conversion, fingerprints without decrypting the private key, remote editing over SSH, and a recursive-descent `ssh_config(5)` parser exposed as an `IConfiguration` source. Released through GitHub Actions to GitHub, winget and the AUR.

### [KnowYourEgk](https://github.com/frequency403/KnowYourEgk) · Rust · egui

Reads the insurance master data (VSD) from a German health insurance card (eGK G2.1), contact or contactless over NFC. Implements PACE (ECDH Generic Mapping, brainpoolP256r1) and AES Secure Messaging following the gematik specifications and ICAO Doc 9303-11, structured as a Rust workspace with a transport abstraction over PC/SC. No network code; the CAN and all session keys are zeroized after use. Releases are cut automatically from the version in `Cargo.toml` once CI on `main` is green.

<a href="https://github.com/frequency403/KnowYourEgk">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/frequency403/KnowYourEgk/main/docs/screenshots/result-dark.png">
    <img alt="KnowYourEgk showing the insurance data of a health card after a contactless read (example data)" src="https://raw.githubusercontent.com/frequency403/KnowYourEgk/main/docs/screenshots/result-light.png" width="720">
  </picture>
</a>

### [OpenSourceInitiative.LicenseApi](https://github.com/frequency403/OpenSourceInitiative.LicenseApi) · C# · NuGet

.NET client for the Open Source Initiative License API: list, search and filter OSI Approved Licenses® by SPDX ID, name, keyword or steward, including the license text. Multi-targeted and published on [NuGet](https://www.nuget.org/packages/OpenSourceInitiative.LicenseApi).

### Also built

- **[AnyBookStore](https://github.com/frequency403/AnyBookStore)** · C# · ASP.NET Core + Angular: self-hosted personal book library; scan or enter an ISBN, rate it, mark it read, backed by the Open Library catalog
- **[license-me](https://github.com/frequency403/license-me)** · Rust · CLI (archived): creates licenses for unlicensed projects on your machine; predecessor of **[LicenseMe](https://github.com/frequency403/LicenseMe)** (Avalonia)

## Tech stack

| | |
|---|---|
| **Languages** | C#, Rust, PowerShell, Bash, SQL |
| **CI/CD** | GitLab CI, Jenkins, GitHub Actions |
| **Packaging** | NuGet, winget, AUR, NSIS |
| **.NET** | Avalonia, WPF, WinForms, ASP.NET Core, ReactiveUI, DynamicData, Microsoft.Extensions.\* (Hosting, DI, Options), DryIoc, Dapper, EF Core, xUnit |
| **Rust** | egui / eframe, Cargo workspaces |
| **Smart cards and security** | PC/SC, ISO 7816-4, PACE, Secure Messaging, BouncyCastle, MIFARE Classic |
| **Data and APIs** | SQLite, REST, SOAP |
| **Tools** | JetBrains Rider, Jira, Confluence |

## Background

- Certified IT specialist for application development (*Fachinformatiker für Anwendungsentwicklung*)
- Trainer aptitude certificate (*AdA-Schein*, AEVO), 2026
- Languages: German (native), English (fluent)

## Contact

[LinkedIn](https://linkedin.com/in/oliver-schantz-a68356298) · [Reddit](https://reddit.com/user/frequency403)
