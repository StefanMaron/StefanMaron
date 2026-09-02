# Hey, I'm Stefan 👋

```bash
$ whoami
Stefan Maroń — Independent Business Central Developer · Microsoft MVP

$ history | tail -3
2016  started on NAV, back in the C/AL era
2022  went independent
2024  named Microsoft MVP for Business Central

$ ls credentials/
LinterCop.al  BCQF.md  linux-since-2023.log
```

Before the code, I trained in accounting and business organization — that's part of why I still think in posting flows and cost centers before I think in code, and part of why I keep pushing BC into places Microsoft didn't design it to run.

[![Website](https://img.shields.io/badge/stefanmaron.com-blog-0078d4)](https://stefanmaron.com)
[![Consulting](https://img.shields.io/badge/stefanmaronconsulting.com-services-2ea44f)](https://stefanmaronconsulting.com)
[![X](https://img.shields.io/badge/X-%40StefanMaron-000000?logo=x&logoColor=white)](https://x.com/StefanMaron)
[![Bluesky](https://img.shields.io/badge/Bluesky-follow-1185FE?logo=bluesky&logoColor=white)](https://bsky.app/profile/stefanmaron.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/stefan-maron-709928206/)
[![YouTube](https://img.shields.io/badge/YouTube-live_coding-FF0000?logo=youtube&logoColor=white)](https://www.youtube.com/@stefanmaron)

---

## 🔭 Currently

- 🔨 **Building** — test coverage and a watch mode for [AL Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner) (v2.3), and tightening up the BCQF methodology behind my code reviews
- 🌱 **Exploring** — grounding AI coding agents in real BC source with [bc-code-atlas](https://github.com/StefanMaron/bc-code-atlas), an MCP server for AL dependency and implementation lookups
- 💬 **Ask me about** — running BC on Linux, fast AL test pipelines, or static analysis for AL

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
> Run AL unit tests without a BC service tier, Docker, or SQL Server. Transpiles your AL to C# via the BC compiler's public API, rewrites BC runtime types to in-memory mocks with Roslyn, and executes test codeunits directly — once dependencies are downloaded and the app is compiled, each test run itself takes milliseconds.

```bash
dotnet tool install --global MSDyn365BC.AL.Runner
al-runner ./src ./test
# first run downloads dependencies and compiles — later runs are near-instant
```

```
Pull Request
  │
  ├─ al-runner          (seconds)  — catches AL logic bugs fast
  └─ Full BC pipeline   (45+ min)  — full fidelity, only when needed
```

### [bc-code-atlas](https://github.com/StefanMaron/bc-code-atlas)
> A queryable window into BC's AL source and official docs — semantic search, a structural call graph, and dependency lookups behind one MCP endpoint. Point a coding agent at it and ask where BC validates a sales order before posting, or what subscribes to a given event, and get an answer grounded in Microsoft's actual base-application source, not a guess from training data.

---

## 🔧 More tools

| Project | What it does | Stars |
|---|---|---|
| [MSDyn365BC.Sandbox.Code.History](https://github.com/StefanMaron/MSDyn365BC.Sandbox.Code.History) | Builds on sandbox artifacts instead of on-prem, so it picks up hotfixes and updates daily | ![Stars](https://img.shields.io/github/stars/StefanMaron/MSDyn365BC.Sandbox.Code.History?style=social) |
| [MSDyn365BC.Code.History](https://github.com/StefanMaron/MSDyn365BC.Code.History) | The original on-prem source history, updated monthly | ![Stars](https://img.shields.io/github/stars/StefanMaron/MSDyn365BC.Code.History?style=social) |

---

## 💼 Work with me

I do independent Business Central consulting for BC partners and ISVs across Europe — see [stefanmaronconsulting.com](https://stefanmaronconsulting.com) for details.

- **Extension code review** — 5–10 days, with an optional compliance report against ISO/IEC 5055
- **Custom AL development & third-party integrations** — banking, e-commerce, field service, business automation — project or retainer, EU-wide
- **Developer training** — AL fundamentals, upgrade-safe patterns, AI-assisted workflows — half-day or full-day, for teams of 2–10
- **DevOps & tooling** — GitHub Actions / AL-Go setup, static analysis wired into CI as a quality gate

I also wrote the [Business Central Quality Framework](https://stefanmaronconsulting.com/iso-5055-business-central/#bcqf) (BCQF), a versioned extension of ISO/IEC 5055:2021 for AL and Business Central, and I'm the original author of [LinterCop](https://github.com/StefanMaron/BusinessCentral.LinterCop), the first community-driven AL static analyzer (now part of the broader ALCops initiative).

---

## 🛠 Stack

![AL](https://img.shields.io/badge/AL-Business_Central-0078d4?style=flat-square)
![C#](https://img.shields.io/badge/C%23-.NET-512BD4?style=flat-square&logo=dotnet)
![Docker](https://img.shields.io/badge/Docker-Linux_BC-2496ED?style=flat-square&logo=docker)
![PowerShell](https://img.shields.io/badge/PowerShell-Automation-5391FE?style=flat-square&logo=powershell)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI%2FCD-2088FF?style=flat-square&logo=github-actions)

---

## 📈 Activity

### 📊 By the numbers

Public GitHub activity — my own repos and contributions to others, refreshed daily. Commit counts run through a lot of AI-assisted sessions these days, so treat them as an activity signal, not a productivity one.

<!-- stats:START -->
| Commits (public) | PRs opened | PRs merged | Issues opened | Stars earned |
|---|---|---|---|---|
| 3285 | 841 | 795 | 1013 | 909 |
<!-- stats:END -->

### 🕒 Recent activity

<!--START_SECTION:activity-->
1. 🗣 Commented on [#17](https://github.com/StefanMaron/BusinessCentral.BakReader/issues/17#issuecomment-5482877107) in [StefanMaron/BusinessCentral.BakReader](https://github.com/StefanMaron/BusinessCentral.BakReader)
2. 🔒 Closed issue [#2268](https://github.com/StefanMaron/BusinessCentral.AL.Runner/issues/2268) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
3. 🔒 Closed issue [#2270](https://github.com/StefanMaron/BusinessCentral.AL.Runner/issues/2270) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
4. 🎉 Merged PR [#2275](https://github.com/StefanMaron/BusinessCentral.AL.Runner/pull/2275) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
5. 🗣 Commented on [#2259](https://github.com/StefanMaron/BusinessCentral.AL.Runner/issues/2259#issuecomment-5483134904) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
6. ❗ Opened issue [#2268](https://github.com/StefanMaron/BusinessCentral.AL.Runner/issues/2268) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
7. ℹ️ Labeled PR [#2275](https://github.com/StefanMaron/BusinessCentral.AL.Runner/pull/2275) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
8. 💪 Opened PR [#2275](https://github.com/StefanMaron/BusinessCentral.AL.Runner/pull/2275) in [StefanMaron/BusinessCentral.AL.Runner](https://github.com/StefanMaron/BusinessCentral.AL.Runner)
<!--END_SECTION:activity-->

### 📝 Latest posts from [stefanmaron.com](https://stefanmaron.com)

<!-- blog:START -->
- [AL Runner v2.2 and v2.3: Coverage, Quick Scripts, and a Watch Mode You Can Trust](https://stefanmaron.com/posts/al-runner-coverage-execute-and-a-guard-that-worked/)

- [I Can Turn Off My Code. I Can&#39;t Turn Off Yours.](https://stefanmaron.com/posts/modify-deserves-the-same-rule-as-validate/)

- [Weekly Recap: August 7-14](https://stefanmaron.com/posts/weekly-recap-2026-08-14/)

- [AL Runner v2: What Feedback Told Me v1 Was Missing](https://stefanmaron.com/posts/al-runner-v2-emit-through-bc/)
<!-- blog:END -->

### 🎥 Latest from my [live-coding channel](https://www.youtube.com/@stefanmaron)

<!-- youtube:START -->
- [How Good Can AL Code Get? — A Live ISO 5055 Review](https://www.youtube.com/watch?v=JI5KlMxrtoA)

- [Swappable Claude Profiles: Per-Project Configs via Container Mounting &lpar;Part 3&rpar;](https://www.youtube.com/watch?v=LuAHCXiwYn4)
<!-- youtube:END -->

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

- 🌐 [stefanmaron.com](https://stefanmaron.com) — blog
- 🧰 [stefanmaronconsulting.com](https://stefanmaronconsulting.com) — consulting services
- 🐦 [@StefanMaron](https://x.com/StefanMaron) on X
- 🦋 [@stefanmaron.com](https://bsky.app/profile/stefanmaron.com) on Bluesky
- 💼 [LinkedIn](https://www.linkedin.com/in/stefan-maron-709928206/)
- 🎥 [YouTube](https://www.youtube.com/@stefanmaron) — irregular live-coding streams

---

*If you're doing BC development and want faster feedback loops or a Linux-native stack — you're in the right place.*

![Profile Views](https://komarev.com/ghpvc/?username=StefanMaron&label=Profile%20views&color=0078d4&style=flat)
