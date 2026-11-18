# 👋🧩 heval patches

<p align="center">
  <a href="https://morphe.software/add-source?github=heval99/Heval-Morphe-Patches">
    <img src="https://img.shields.io/badge/%E2%9E%95%20%20Add%20to%20Morphe-1E5AA8?style=for-the-badge" height="46" alt="Add to Morphe">
  </a>
  <br>
  <sub>One tap adds this patch source to Morphe Manager</sub>
</p>

<p align="center">
  <a href="https://github.com/heval99/Heval-Morphe-Patches/releases/latest"><img src="https://img.shields.io/github/v/release/heval99/Heval-Morphe-Patches?label=stable&color=2ea44f" alt="Latest stable release"></a>
  <a href="https://github.com/heval99/Heval-Morphe-Patches/releases"><img src="https://img.shields.io/github/v/release/heval99/Heval-Morphe-Patches?include_prereleases&label=pre-release&color=orange" alt="Latest pre-release"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-GPLv3-blue" alt="GPLv3"></a>
  <a href="https://ko-fi.com/heval99"><img src="https://img.shields.io/badge/Support%20me%20on-Ko--fi-72a4f2?logo=ko-fi&logoColor=white" alt="Support me on Ko-fi"></a>
  <a href="https://paypal.me/HevalXode"><img src="https://img.shields.io/badge/Donate-PayPal-00457C?logo=paypal&logoColor=white" alt="Donate with PayPal"></a>
</p>

Custom [Morphe](https://morphe.software) patches by heval99 for apps I use: ad removal,
telemetry blocking and premium/licence unlocks for sports, music, notes, email, maps and
utility apps.

## 🚀 Quick start

1. Install [Morphe Manager](https://morphe.software).
2. Tap **[Add to Morphe](https://morphe.software/add-source?github=heval99/Heval-Morphe-Patches)**,
   or add this repository as a patch source by hand:
   `https://github.com/heval99/Heval-Morphe-Patches`
3. Pick the app, choose the patches you want and patch.

**Stable or pre-release?** The stable channel follows the
[latest release](https://github.com/heval99/Heval-Morphe-Patches/releases/latest). Turn on
**Pre-release patches** for this source in Morphe Manager to get fixes and new apps a few days
earlier.

## 🩹 Patches list

Each app lists the versions its patches were verified on (shown in Morphe Manager). Other
versions may work but aren't guaranteed; if an app update breaks a patch,
[open an issue](https://github.com/heval99/Heval-Morphe-Patches/issues/new/choose).

<!-- PATCHES_START EXPANDED -->
> **[v4.0.0-dev.1](https://github.com/kinoosaki/Heval-Morphe-Patches/releases/tag/v4.0.0-dev.1)**&nbsp;&nbsp;•&nbsp;&nbsp;`dev`&nbsp;&nbsp;•&nbsp;&nbsp;**1** apps&nbsp;&nbsp;•&nbsp;&nbsp;**2** patches&nbsp;&nbsp;•&nbsp;&nbsp;updated 2026-11-18

🚫 ads&nbsp;&nbsp;🛡️ telemetry / tracking&nbsp;&nbsp;💎 premium / pro&nbsp;&nbsp;🔑 license check&nbsp;&nbsp;🔕 prompts / notifications&nbsp;&nbsp;🧪 experimental

📝 Productivity & notes

#### 📝 Productivity & notes <sub>1 app</sub>

| | App | Patches | Latest verified | Type | Google Play |
|:-:|---|---|---|:-:|:-:|
| <img src="assets/icons/net.dinglisch.android.taskerm.png" width="20" height="20" alt=""> | **Tasker** | 💎 🧩 2 | `6.7.8` | APK | [Play](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm) |

### 🔍 Patch details

#### 📝 Productivity & notes

<details>
<summary><img src="assets/icons/net.dinglisch.android.taskerm.png" width="16" height="16" alt=""> <b>Tasker</b> &nbsp;·&nbsp; 2 patches &nbsp;·&nbsp; <code>net.dinglisch.android.taskerm</code></summary>

Verified on: `6.7.8`

| Patch | What it does | Default |
|---|---|:-:|
| 💎 **Enable Full Version** | Unlocks the full version. | ✅ |
| 🧩 **GmsCore support** | Lets you sign in with Google through MicroG RE. | ➖ |

</details>

<sub>✅ on by default&nbsp;&nbsp;➖ off by default (enable it in Morphe Manager)</sub>
<!-- PATCHES_END -->

### 🧪 Experimental patches

Some patches are marked **experimental** in Morphe Manager (for example Brave's *Disable
telemetry*, *Disable ads* and *Hide promotional prompts*). They are tested but newer, so
they are **off by default**; enable them yourself and report anything odd.

## ⚠️ Good to know

- **Only what the app decides locally can be unlocked.** Features served or checked by the
  developer's servers (cloud content, AI features, VPN servers, server-enforced limits) stay
  locked; patches don't fake them. Patch descriptions say when something is only partly
  unlocked.
- **Google sign-in may break.** Patched apps are re-signed, so "Sign in with Google" and some
  other Google services can stop working. Use email login where the app offers it.
- **Push notifications** in some apps need [MicroG](https://github.com/microg/GmsCore) with
  signature spoofing after patching.
- **LibrePods is not patched any more.** At the developer's request, use the free FOSS build
  from the [LibrePods releases](https://github.com/librepods-org/librepods/releases) instead;
  it needs no patch.
- **Use the APK type Morphe Manager suggests.** Some apps are only published as split bundles
  (APKM); patch the full bundle, not just the base APK.

## 💬 Requests and bug reports

- **Something broke?** Open a
  [bug report](https://github.com/heval99/Heval-Morphe-Patches/issues/new/choose) with the app
  version, the patch bundle version and what you see.
- **Want an app patched?** Open a thread in the
  [Requests discussions](https://github.com/heval99/Heval-Morphe-Patches/discussions/categories/requests)
  (search first, and check the
  [blocklist](https://github.com/heval99/Heval-Morphe-Patches/blob/dev/docs/patch-blocklist.md)
  for apps that cannot be patched), or email hevalomevalo@gmail.com.

## 🤖 How the patches are made

> **AI-generated patches.** Every patch here is written with AI assistance: the code
> analysis, patch code and smoke tests are AI-generated. Before each release they are
> verified by applying them to the real APKs (smoke tests in `patches/src/test/`) and
> checking the patched code. Review before use; no warranty.

## 🛠️ Building

```
./gradlew :patches:buildAndroid
```

The bundle is written to `patches/build/libs/`. The Morphe Gradle plugin is downloaded from
GitHub Packages, so set `GITHUB_ACTOR` and `GITHUB_TOKEN` (a token with `read:packages`)
first. See the [Morphe documentation](https://github.com/MorpheApp/morphe-documentation) for
details.

## 🔗 Other projects

- **[Sideport](https://github.com/heval99/Sideport)**: a userscript that adds a **Get APK**
  button to every Google Play app page. It downloads directly from 6 sources with live
  availability checks and shows when Morphe patches exist for the app. No tracking.
  [Install it](https://github.com/heval99/sideport/raw/main/sideport.user.js) with
  Tampermonkey or Violentmonkey.

## 💙 Support

If these patches are useful to you, you can support the work:

[![Support me on Ko-fi](https://img.shields.io/badge/Support%20me%20on-Ko--fi-72a4f2?logo=ko-fi&logoColor=white&style=for-the-badge)](https://ko-fi.com/heval99)
[![Donate with PayPal](https://img.shields.io/badge/Donate-PayPal-00457C?logo=paypal&logoColor=white&style=for-the-badge)](https://paypal.me/HevalXode)

## 📜 License

heval patches are licensed under the [GNU General Public License v3.0](LICENSE).
