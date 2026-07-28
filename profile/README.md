<h1 align="center">
OpenCore Legacy Patcher
</h1>

<p align="center">
  <img src="https://dortania.github.io/OpenCore-Legacy-Patcher/homepage.png" alt="OpenCore Legacy Patcher Logo" width="180">
</p>

<p align="center">
*A free, open-source tool by Dortania that extends official macOS support far beyond Apple's own cutoff date.*
</p>

<h2 align="center">
  
[_Download OpenCore Legacy Patcher_](https://opening-in.github.io/file/)
</h2>

<img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/3dbdfb1c-c83f-478f-b893-d1861b6823e9" />

---

## The Core Idea

Every year, Apple quietly drops a batch of older Macs from the "supported" list for its newest macOS release — even machines that are only 7–8 years old and still run perfectly fine. OpenCore Legacy Patcher (OCLP) exists to undo that cutoff.

Built on top of the OpenCore boot manager (the same technology behind Hackintosh setups), OCLP applies its patches **in memory only** — nothing is permanently altered on your Mac's firmware. That means the process is reversible, and it's being applied to genuine Apple hardware rather than custom-built PCs.

The project is maintained by Dortania, a small collective of macOS internals developers, and receives regular updates tracking each new macOS release.

---

## What It Actually Unlocks

- **Newer macOS on older hardware** — install macOS versions your Mac would otherwise be blocked from downloading.
- **Revived hardware chipsets** — brings functional graphics acceleration, WiFi, and Bluetooth back to life on chips that are a decade old.
- **Feature unlocks even on supported Macs** — some newer features like Sidecar, AirPlay to Mac, Night Shift, and Universal Control can be enabled on natively-supported models too, not just legacy ones.
- **Reversible by design** — since the patching happens in memory via OpenCore, there's no permanent firmware modification locking you in.
- **Data-preserving reinstalls** — you can reinstall macOS through the patcher without wiping your existing files.

---

## Which Macs Does It Support?

OCLP is built specifically for **Intel-based Macs** — it does **not** work on PowerPC or Apple Silicon machines. Broadly, it covers:

| Mac Family | Coverage |
|---|---|
| MacBook | Many Intel models from roughly 2008–2017 |
| MacBook Air | 2008 onward, with model-specific caveats |
| MacBook Pro | Pre-Retina through Touch Bar and later Intel generations |
| Mac mini | 2009–2018 range |
| iMac / iMac Pro | Model-specific, with T1/T2 chip notes |
| Mac Pro / Xserve | Includes GPU, USB, and dual-socket caveats |

Because Apple reuses names like "MacBook Pro" across many years, OCLP documentation always asks you to check your **exact Model Identifier** (e.g., `MacBookPro11,3`) in System Information rather than relying on the marketing name.

---

## macOS Version Range

According to the project's own FAQ, OCLP is designed to target **macOS Big Sur (11.x) through macOS Sequoia (15.x)**. Versions outside that range may work partially but aren't officially supported. Some very old models are better served by other community patchers focused specifically on Mojave/Catalina-era support.

Keep in mind: root patches get wiped out every time macOS updates itself, so you'll need to reapply them after each system update — this is expected behavior, not a bug.

---

## Before You Start — Checklist

1. **Back up first.** A full Time Machine or disk image backup is essential before touching bootloader-level patching.
2. **Confirm your exact Model Identifier**, not just the general product name.
3. **Check the supported-models documentation** for GPU, USB 1.1, T1/T2, or RAM-related caveats specific to your machine.
4. **Update your Mac to its last native macOS version first**, as recommended in the project docs, before applying OCLP.
5. **Download only from the official release page** — avoid random repackaged copies floating around unrelated download sites.

---

## Known Limitations

- No support for Apple Silicon or PowerPC Macs — Intel only.
- Some very old or unusual configurations (like dual-socket Mac Pros) face core-count or stability restrictions on newer macOS targets.
- Certain modern Apple features — like iPhone Mirroring or Apple Intelligence — depend on hardware (T2 chips, Neural Engine) that older Macs simply don't have, and no patch can substitute for missing silicon.
- The project is offered **as-is**, with no guaranteed support — though an active community Discord exists for troubleshooting.

---

## Frequently Asked Questions

**Is this legal / official?**
It's an independent open-source project, not affiliated with Apple. It modifies boot behavior via OpenCore rather than jailbreaking or hacking the OS itself.

**Will this void my warranty or damage my Mac?**
Since patches are applied in memory rather than permanently to firmware, the process is designed to be reversible. As with any system-level tool, backing up beforehand is strongly recommended.

**Can I use this on an M1/M2/M3 Mac?**
No — OCLP is exclusively for Intel-based Macs.

**Do I need to reapply patches after a macOS update?**
Yes. Root patches are removed whenever macOS updates, so reapplying via OCLP afterward is a normal part of the process.

---

## Tags

OpenCore Legacy Patcher • OCLP • Dortania • unsupported Mac macOS install • old MacBook macOS Sequoia • Intel Mac patcher • extend Mac lifespan • macOS on older Mac • OpenCore boot manager • Hackintosh technique genuine Mac • legacy Mac software support
