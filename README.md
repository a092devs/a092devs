# a092devs

**Android & full-stack engineer**

Two kinds of work: runtime instrumentation for Android apps, and the data-in →
dashboard-out path on the web. The common thread is software that has to keep working
when something underneath it changes.

## Projects

| Project | Stack | What it does |
| --- | --- | --- |
| **[NexFusion](https://github.com/a092devs/NexFusion)** | Kotlin · Compose · libxposed · DexKit | Applies bytecode patches to installed apps in memory — no re-signing, no reinstall |
| **[Nexfusion-Patches](https://github.com/a092devs/Nexfusion-Patches)** | Kotlin | The signed `.nxb` bundles NexFusion loads, one per target app |
| **[OpsVista](https://github.com/a092devs/OpsVista)** | React · FastAPI · PostgreSQL | Operations dashboard over a garden-retailer dataset |
| **[DataFoundry](https://github.com/a092devs/DataFoundry)** | React · FastAPI · PostgreSQL | Upload a CSV, profile it, validate it, explore it |

## NexFusion

Ahead-of-time patchers decompile the target, modify it, re-sign it and reinstall it.
NexFusion does none of that: hooks attach **in memory at process start**, so the app on
disk stays the official build and keeps its Play Store signature and Play Protect
status.

- **Symbol resolution, not offsets** — DexKit finds obfuscated classes and methods by
  bytecode opcode patterns and string fingerprints, so a patch survives an app update
  that would break a hardcoded offset
- **Blast radius** — every hook runs inside a guarded boundary; a symbol that moves
  degrades one feature instead of crashing the host app
- **`.nxb` bundles** — signed containers loaded into process memory, never installed as
  apps, distributed from [Nexfusion-Patches](https://github.com/a092devs/Nexfusion-Patches)
- **Carve-out by design** — banking, payment and security-critical apps are excluded
  from patching regardless of what a bundle asks for

Targets include YouTube, Reddit, Instagram, Facebook, Telegram, X and Maps. Needs
Android 8.1+ (API 27) with root and a `libxposed` API 101 framework.

> [!IMPORTANT]
> Patch bundles execute bytecode inside other applications' processes. Install them only
> from maintainers you trust.

## The dashboard pair

OpsVista and DataFoundry share a shape: files in, PostgreSQL behind a FastAPI service,
React on top.

**OpsVista** is fixed to one supplied garden-retailer dataset — seven Parquet tables —
and charts sales, orders, customers, products, payments, returns and shipping time, with
a persisted dark/light choice.

**DataFoundry** is the generalised version: upload any CSV and get column profiles and
quality checks before exploring it. It grew out of an Olist marketplace analysis
(99K orders, 16.01M revenue, 91.9% delivered on time or early), but that multi-table
work and its Power BI report are **not** what the current app does — it handles one CSV
per upload and does not join separate tables.

## Contact

[LinkedIn](https://www.linkedin.com/in/a092devs) ·
[all repositories](https://github.com/a092devs?tab=repositories)
