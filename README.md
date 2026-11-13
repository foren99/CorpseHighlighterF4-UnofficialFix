# ⚠️ TESTED FOR 4-5 HOURS - WORK IN PROGRESS ⚠️
**This build has been tested for 4-5 hours of continuous gameplay without any crashes. However, it is still an unofficial build. Use at your own risk and always keep a backup of your save files.**

---

# Corpse Highlighter F4 - Unofficial Bugfix Fork

This is an **unofficial bugfix fork** of the original [CorpseHighlighterF4](https://github.com/Into-The-Rough/CorpseHighlighterF4) mod.

**All credit for the original mod and base code goes to the original creator (Into-The-Rough / lNexAl).** This fork was created merely as a community patch to address a few known bugs reported by users.

## 🛠️ What was fixed in this fork?

1. **Rapid Deaths (Missing Highlights):** Added a retry mechanism. If the 3D model (ragdoll) of a corpse isn't ready immediately after death, the plugin will now retry applying the shader for a few frames instead of giving up instantly.
2. **Save/Load (Reload) Bug:** Fixed the issue where corpses would remain highlighted forever if you saved and reloaded the game before looting them. A "fallback" mechanism ensures the shader is forcefully removed when the player interacts with the corpse, even if the plugin's memory was reset after loading.
3. **Empty Corpses (Partial Fix):** Corpses with no items used to glow indefinitely. While an initial inventory check is not possible due to an old `commonlibf4` limitation, a **fallback mechanism** now ensures that the glow is **forcefully removed** as soon as the player presses the **R (Transfer) key** on an empty corpse. The glow will not persist indefinitely.
4. **100% Safe to Uninstall (Zero Save Bloat):** The plugin **does NOT** use F4SE Serialization (co-saves). It writes absolutely zero custom data to your save file. You can safely remove this mod at any time without corrupting your save.

## 📦 Installation

1. Ensure you have the original mod's base files installed (MCM, Config folder, etc.).
2. Download the latest `CorpseHighlighterF4.dll` from the **Releases** section on the right.
3. Replace the old `.dll` file in your `Fallout 4\Data\F4SE\Plugins\` folder with the new one.
4. (Optional) You can safely delete the old `.pdb` file from the original mod.

## ⚠️ Disclaimer

This is an unofficial community patch. **Please do not report bugs or issues from this specific fork to the original mod author.** If you encounter any problems with this test build, please open an "Issue" here on this GitHub repository.
