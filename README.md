# a092devs

**Android & full-stack engineer**

Android apps and system tooling in Kotlin, services in Python and Node, frontends in
React, PostgreSQL for storage.

## Projects

| Project | Stack | What it does |
| --- | --- | --- |
| **[NexFusion](https://github.com/a092devs/NexFusion)** | Kotlin · Jetpack Compose · libxposed · DexKit | Applies runtime bytecode patches to installed apps |
| **[Nexfusion-Patches](https://github.com/a092devs/Nexfusion-Patches)** | Kotlin | Signed `.nxb` patch bundles that NexFusion loads |
| **[OpsVista](https://github.com/a092devs/OpsVista)** | React · FastAPI · PostgreSQL | Dashboard over a retail operations dataset |
| **[DataFoundry](https://github.com/a092devs/DataFoundry)** | React · FastAPI · PostgreSQL | CSV upload, validation and analytics |

## NexFusion

A patch manager for rooted Android devices. It uses LSPosed / libxposed (API 101) to
apply bytecode patches to other apps as they start. The target APK is not modified on
disk, so it keeps its original signature and Play Protect status.

- Patches ship as signed `.nxb` bundles loaded into process memory, not installed as
  apps. They come from [Nexfusion-Patches](https://github.com/a092devs/Nexfusion-Patches).
- Obfuscated class and method names are resolved at runtime with DexKit, using bytecode
  opcode patterns and string fingerprints. Fixed offsets would break on the next app
  update; pattern matching usually does not.
- Each hook runs inside error handling, so a patch that fails to resolve leaves that one
  feature off instead of crashing the host app.
- Banking, payment and security-critical apps are excluded from patching.

Supported targets include YouTube, Reddit, Instagram, Facebook, Telegram, X and Maps.
Requires Android 8.1+ (API 27) and root.

## OpsVista

Seven Parquet tables of garden retail data are loaded into PostgreSQL, served by a
FastAPI backend and displayed in a React dashboard covering sales, orders, customers,
products, payments, returns and shipping time. Dark and light themes, with the choice
remembered per browser.

## DataFoundry

Upload a CSV and the app profiles its columns, runs validation checks, stores the
dataset in PostgreSQL and lets you explore it. FastAPI backend, React frontend.

It began as an analysis of the Olist Brazilian e-commerce dataset (99K orders, 91.9%
delivered on time or early) feeding a Power BI report. That version is gone: the current
app takes one CSV at a time and does not join separate tables.

## Contact

[LinkedIn](https://www.linkedin.com/in/a092devs) ·
[all repositories](https://github.com/a092devs?tab=repositories)
