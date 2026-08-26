# Hey, I'm Stefan 👋

**Microsoft Dynamics 365 Business Central Developer · Microsoft MVP · Freelance**

I push BC into places Microsoft didn't design it to go — Linux, in-memory test execution, and fast CI pipelines.

[![Website](https://img.shields.io/badge/stefanmaron.com-blog-0078d4)](https://stefanmaron.com)
[![X](https://img.shields.io/badge/X-%40StefanMaron-000000?logo=x&logoColor=white)](https://x.com/StefanMaron)
[![Bluesky](https://img.shields.io/badge/Bluesky-follow-1185FE?logo=bluesky&logoColor=white)](https://bsky.app/profile/stefanmaron.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/stefan-maron-709928206/)

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
| [MSDyn365BC.Code.History](https://github.com/StefanMaron/MSDyn365BC.Code.History) | Full BC source history, updated monthly — diff any version | ![Stars](https://img.shields.io/github/stars/StefanMaron/MSDyn365BC.Code.History?style=social) |
| [BusinessCentral.LinterCop](https://github.com/StefanMaron/BusinessCentral.LinterCop) | Community-driven AL linter — catch issues before they ship | ![Stars](https://img.shields.io/github/stars/StefanMaron/BusinessCentral.LinterCop?style=social) |
| [BusinessCentral.Sentinel](https://github.com/StefanMaron/BusinessCentral.Sentinel) | Security & quality scanner for BC extensions | ![Stars](https://img.shields.io/github/stars/StefanMaron/BusinessCentral.Sentinel?style=social) |

---

## 🛠 Stack

![AL](https://img.shields.io/badge/AL-Business_Central-0078d4?style=flat-square)
![C#](https://img.shields.io/badge/C%23-.NET-512BD4?style=flat-square&logo=dotnet)
![Docker](https://img.shields.io/badge/Docker-Linux_BC-2496ED?style=flat-square&logo=docker)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat-square&logo=powershell)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?style=flat-square&logo=github-actions)

---

## 📈 Activity

<!--START_SECTION:activity-->
<!--END_SECTION:activity-->

### 📝 Latest posts from [stefanmaron.com](https://stefanmaron.com)

<!-- blog:START -->
<!-- blog:END -->

<details>
<summary>📊 <b>GitHub stats</b></summary>
<br>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=StefanMaron&theme=github_dark">
  <img alt="Profile summary" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=StefanMaron&theme=default">
</picture>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=StefanMaron&theme=github_dark">
  <img alt="Top languages" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=StefanMaron&theme=default">
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=StefanMaron&theme=github_dark">
  <img alt="Most committed language" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=StefanMaron&theme=default">
</picture>

</details>

---

## 📬 Find me

- 🌐 [stefanmaron.com](https://stefanmaron.com)
- 🐦 [@StefanMaron](https://x.com/StefanMaron) on X
- 🦋 [@stefanmaron.com](https://bsky.app/profile/stefanmaron.com) on Bluesky
- 💼 [LinkedIn](https://www.linkedin.com/in/stefan-maron-709928206/)

---

*If you're doing BC development and want faster feedback loops or a Linux-native stack — you're in the right place.*

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=StefanMaron&label=Profile%20views&color=0078d4&style=flat)

</div>
