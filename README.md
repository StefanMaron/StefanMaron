# Hey, I'm Stefan 👋

**Microsoft Dynamics 365 Business Central Developer · Microsoft MVP · Freelance**

I push BC into places Microsoft didn't design it to go — Linux, in-memory test execution, and fast CI pipelines.

---

## 🚀 Cutting-edge projects

### [MsDyn365Bc.On.Linux](https://github.com/StefanMaron/MsDyn365Bc.On.Linux)
> Run the unmodified BC service tier on Linux via a .NET startup hook that redirects Win32 P/Invokes, stubs HttpSys → Kestrel, and patches ~20 Windows-only runtime assumptions — all at boot, without touching a single Microsoft binary.

```bash
git clone https://github.com/StefanMaron/MsDyn365Bc.On.Linux
cd MsDyn365Bc.On.Linux && docker compose up -d --wait
# BC is live in ~5 min. No Windows. No VM.
```

### [BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
> AL unit tests in **milliseconds** — no BC service tier, no Docker, no SQL Server. Transpiles your AL to C# via the BC compiler's public API, rewrites BC runtime types to in-memory mocks with Roslyn, and executes test codeunits directly.

```bash
dotnet tool install --global MSDyn365BC.AL.Runner
al-runner ./src ./test   # runs in < 1 second
```

```
Pull Request
  │
  ├─ al-runner          (seconds)  — catches AL logic bugs fast
  └─ Full BC pipeline   (45+ min)  — full fidelity, only when needed
```

---

## 🔧 More tools

| Project | What it does | Stars |
|---|---|---|
| [MSDyn365BC.Code.History](https://github.com/StefanMaron/MSDyn365BC.Code.History) | Full BC source history, updated monthly — diff any version | ⭐ 471 |
| [BusinessCentral.LinterCop](https://github.com/StefanMaron/BusinessCentral.LinterCop) | Community-driven AL linter — catch issues before they ship | ⭐ 108 |
| [BusinessCentral.Sentinel](https://github.com/StefanMaron/BusinessCentral.Sentinel) | Security & quality scanner for BC extensions | ⭐ 23 |

---

## 🛠 Stack

![AL](https://img.shields.io/badge/AL-Business_Central-0078d4?style=flat-square)
![C#](https://img.shields.io/badge/C%23-.NET-512BD4?style=flat-square&logo=dotnet)
![Docker](https://img.shields.io/badge/Docker-Linux_BC-2496ED?style=flat-square&logo=docker)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat-square&logo=powershell)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?style=flat-square&logo=github-actions)

---

## 📬 Find me

- 🌐 [stefanmaron.com](https://stefanmaron.com)
- 🐦 [@StefanMaron](https://x.com/StefanMaron) on X
- 🦋 [@stefanmaron.com](https://bsky.app/profile/stefanmaron.com) on Bluesky
- 💼 [LinkedIn](https://www.linkedin.com/in/stefan-maron-709928206/)

---

*If you're doing BC development and want faster feedback loops or a Linux-native stack — you're in the right place.*
