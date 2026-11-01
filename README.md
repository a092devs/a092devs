<div align="center">

# Hi, I'm Arsalan 👋

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/typing-dark.gif">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/typing-light.gif">
  <img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/typing-dark.gif" alt="Android, web and data work" width="620" />
</picture>

[**LinkedIn**](https://www.linkedin.com/in/a092devs) &nbsp;·&nbsp; [**X**](https://twitter.com/a092devs) &nbsp;·&nbsp; [**Email**](mailto:arsalanakhtar0@gmail.com)

</div>

---

I build software for Android at the framework level, the web apps and dashboards that
sit around it, and the pipelines that turn what those systems collect into something
readable. Most of my work involves making something behave differently than it shipped,
whether that is a patch bundle for a social app, a module that fixes a bad ROM port, or
a query that reconciles two systems that disagree about an order.

---

### 🧭 What I do

**Android, ROMs and patching**

Xposed and LSPosed module development, Magisk and KernelSU modules, and runtime patch
authoring against real apps rather than source I control. Comfortable reading smali and
dex when the source isn't available, working with AOSP and vendor trees, and debugging
down into telephony and IMS when the symptom is only visible in the status bar. I
currently maintain a port of OxygenOS 16 to the Poco F7, which keeps me close to the
bring-up side of things.

**Web platforms and APIs**

React front ends on FastAPI or Node back ends, with PostgreSQL underneath. I tend to
end up building internal operations tooling rather than marketing sites: dashboards
where someone can actually work out why a shipment is late or a payment never settled.

**Data and analytics**

ETL work in Python, SQL transformations that live in the database rather than in a
notebook, and Power BI or dashboard layers on top. The useful part is usually deciding
what the grain of a fact table should be, not the charting.

---

### 🌟 Selected work

| Project | Details |
|:--|:--|
| **[NexAlloyNext](https://github.com/a092devs/NexAlloyNext)** | LSPosed and Morphe patch manager for Android, written in Kotlin. Ships two complete design systems, Material 3 and MIUIX, and handles patch discovery, installation and updates. |
| **[NexAlloyNext-Patches](https://github.com/a092devs/NexAlloyNext-Patches)** | The patch bundles that run on it, distributed as `.nxb`. Covers Instagram, Facebook, YouTube, PixelBoard Gboard, Proton VPN, Discord and Reddit, and keeps working across app updates without forking the app. |
| **[SystemFixes](https://github.com/a092devs/SystemFixes)** | An LSPosed module that repairs the OxygenOS 16 port on the Poco F7. Fixes a storage capacity reported from the wrong chip, rebuilds the Vo5G indicator so it follows the real voice radio technology per SIM, and only shows 5G+ when the network is genuinely aggregating NR carriers. |
| **[OpsVista](https://github.com/a092devs/OpsVista)** | Ecommerce operations dashboard. React and FastAPI over PostgreSQL, covering sales, orders, customers, payments, returns and shipping times. |
| **[DataFoundry](https://github.com/a092devs/DataFoundry)** | The analytics side of the same store: Python and SQL pipelines feeding a PostgreSQL warehouse and Power BI reporting. |
| **[GameUnlocker](https://github.com/a092devs/GameUnlocker)** | C++ Magisk and KernelSU module that unlocks 90+ FPS frame rates in BGMI and PUBG, tuned to hold up on weaker devices. |
| **[irctc-cypress-automation](https://github.com/a092devs/irctc-cypress-automation)** | Cypress end-to-end automation against the IRCTC booking flow, completing a tatkal booking run in about a minute. |
| **[termux-onyx-setup](https://github.com/a092devs/termux-onyx-setup)** | A modular Termux environment with zsh and Powerlevel10k, packaged so the shell, prompt and tooling can be enabled independently. |

---

### 🤝 Services

Happy to take on work in the areas above, particularly where it needs someone who will
go below the app layer:

- **Android module and patch development.** Xposed and LSPosed modules, Magisk and
  KernelSU work, and reverse-engineering an app's behaviour when there is no source.
- **ROM porting and device bring-up fixes.** Diagnosing what broke when a build moved to
  hardware it wasn't made for, especially telephony, camera and system UI symptoms.
- **Internal dashboards and APIs.** React and FastAPI or Node with PostgreSQL, from the
  data model through to the interface.
- **Data pipelines and reporting.** ETL in Python, warehouse modelling in SQL, and Power
  BI or dashboard layers over the top.

The fastest way to reach me is [email](mailto:arsalanakhtar0@gmail.com).

---

### 🛠️ Stack

<div align="center">

<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/kotlin.png" width="44" height="44" alt="Kotlin" title="Kotlin" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/openjdk.png" width="44" height="44" alt="Java" title="Java" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/cplusplus.png" width="44" height="44" alt="C++" title="C++" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/python.png" width="44" height="44" alt="Python" title="Python" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/fastapi.png" width="44" height="44" alt="FastAPI" title="FastAPI" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/nodedotjs.png" width="44" height="44" alt="Node.js" title="Node.js" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/react.png" width="44" height="44" alt="React" title="React" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/javascript.png" width="44" height="44" alt="JavaScript" title="JavaScript" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/tailwindcss.png" width="44" height="44" alt="Tailwind CSS" title="Tailwind CSS" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/postgresql.png" width="44" height="44" alt="PostgreSQL" title="PostgreSQL" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/docker.png" width="44" height="44" alt="Docker" title="Docker" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/git.png" width="44" height="44" alt="Git" title="Git" />&nbsp;
<img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/icons/linux.png" width="44" height="44" alt="Linux" title="Linux" />

</div>

---

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/stats-dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/stats-light.png">
  <img src="https://raw.githubusercontent.com/a092devs/profile-assets/main/assets/stats-dark.png" alt="GitHub stats" width="420" />
</picture>

</div>
