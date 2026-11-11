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

## Contact

[LinkedIn](https://www.linkedin.com/in/a092devs) ·
[Telegram](https://www.t.me/a092devs) ·
[all repositories](https://github.com/a092devs?tab=repositories)
