# 🔥 RisingOS Version 2.2 (Ignis)

## 🏛️ Introduction
- Embracing the blazing spirit of Ignis, derived from the Latin word for "fire," this release captures our burning passion for innovation.

---

## 🔒 Security Updates
- **Android Security:** Stay protected with up-to-date security patches for April 2024.
---

## 💬 Highlights (RisingOS Exclusive Additions)

For previous changelogs from our initial beta release, please refer to [Beta Release Changelog](https://github.com/RisingTechOSS/risingOS_changelogs/tree/32f1bc41a6a0b7c263b157c68dacd08ce4e768c8).

---

This update brings previous features from the beta releases with the following improvements:
- **Framework:**
  - Rebased on top of crDroid Android Project with risingOS additions on top (Big thanks and credits to crDroid Android and LineageOS projects for making this release possible)

- **AOSP QPR2 Framework:**
  - Fixed AOD now playing text alignment (when custom weather is enabled).
  - Fixed QuickSettings header icons/text colors for light/dark theme modes.
  - Fixed app drawer prediction row not showing themed icons
  - Fixed Volume panel issues (04/13/24)
  - Improved Freeform handling (for ortus launcher users) (04/13/24)
  - Reworked bluetooth dialog click/tap handling; click to toggle bluetooth, long press to open dialog (04/19/24)
  - Applied workaround for volume ui delays when adjusting volume through volume keys (04/19/24)
  - Fixed notification panel light/dark theme colors (04/21/24)
  - Restored offload/direct audio track support (04/28/24)
  - Aligned A2DP and speaker volume (04/28/24)
  - Optimized low memory killer daemon (05/06/24)
  - Silenced spammy debugging messages that causes battery drain (05/06/24)

- **Adaptive Charging:**
  - Introducing Adaptive Charging, which implements the system's power manager adaptive power management when enabled.
  
- **Audio Effects [BETA]:**
  - Re-introducing Audio Effects as Adaptive Sound Engine with a new look and new adaptive sound modes.
  - Attached audio effects to global output [credits to Gabi Moreno](https://github.com/soygabimoreno) (04/13/24)
  - Improved profiles tunings (04/16/24)
  - Added Sound Engine QS tile and lockscreen widget toggle (05/06/24)

- **Backgrounds:**
  - Imported Nothing 2a wallpapers (04/13/24)

- **Boost Framework:**
  - Reworked boosting framework, utilizing Code-Linaro's (Qualcomm) boosting framework, rewritten to be like Google Pixel's libperfmgr for general compatibility.
  - Integrated boosting framework into Game Space.
  - Made power boosts more efficient (04/22/24)
  - Resolved power regressions (04/28/24)

- **Clock Styles:**
  - Fixed custom clock alignment (04/13/24)

- **Dark Theme:**
  - Introducing True Amoled Dark mode (05/09/24)

- **Depth Wallpaper:**
  - Introducing Depth Wallpaper feature [credits to Siavash](https://github.com/siavash79) (05/06/24)

- **Face Unlock:**
  - Moved face unlock icon indication to top (04/13/24)
  - Added face unlcok icon indication when entering pin/password (04/13/24)
  - Fixed face unlock icon inconsistencies (04/16/24)
  - Add workaround for face unlock timeouts (face unlock unavailable issue) (04/28/24)

- **GameSpace:**
  - Made FPS counter functional (04/19/24)

- **Healthy Charge:**
  - Introducing Healthy Charge Service(05/09/24)

- **Island Notification:**
  - Contacts/contents icons/pictures are now added to the island notification.

- **LockScreen Clock Styles:**
  - Added iOS widget to iOS Clock style; [Big thanks and credits to DrDisagree](https://github.com/Mahmud0808)
  - Improved and resolved UI performance regressions.

- **LockScreen Widgets [BETA]:**
  - New swipe left/right media playback navigation support for big media widget
  - Lockscreen widgets can now be added to the default clock style.
  - Fixed and improve media widget playback ui (04/13/24)
  - Added wifi, data, ringer toggle widgets (04/21/24)
  - Reduced small widgets padding (04/21/24)
  - Added bluetooth toggle widget (04/22/24)
  - Improved toggle widgets state listening (04/22/24)
  - Fixed lockscreen widgets preview layout (04/22/24)
  - Added expand on long press support to some widgets (04/28/24) 
  - Fixed scaling on high dpi devices (05/06/24)

- **Memory Optimization:**
  - Improved memory management by porting Code-Linaro's Low-Memory-Killer Daemon tweaked and enhanced by [arter97](https://github.com/arter97/).

- **Ortus Launcher:**
  - Rebased on top of crDroid Home
  - Added support for third party themed icon packs and forced monochrome icons.
  - Improved themed/forced monochrome icons rendering and support
  - Revamped recents overview panel 
  - Freeform tasks launched from shortcut now stays on top even after launching a new app
  - Updated to material design (04/16/24)
  - Updated themed icons redirect to lawnicons release page (04/16/24)
  - Prevented themed icons icon pack/s from showing on icon packs section (04/19/24)
  - Fixed Free memory calculation (05/06/24)
  - Restored homescreen popup legacy order (05/06/24)
  - Updated search bar colors (05/06/24)
  - Added force kill option to system shortcut (05/06/24)

- **Pixel Framework:**
  - Introducing Ported Pixel features such as Smartspace, Ambient Music, Reverse Charging; [credits to Pixel Experience Project for the base framework](https://github.com/PixelExperience)

- **Pocket Mode:**
  - Added accidental phone wakeup handling mechanism.
  - Improved power button and call handling (04/13/24)
  - Introducing Always on Pocket mode (04/28/24)

- **QS Header Image:**
  - QS Header icons/text colors now changes to white when QS Header Image is enabled.

- **RisingUI:**
  - Added long press functionality to per-app volume button.
  - Introducing nothing breathing UDPS icon style.
  - Reworked lockscreen shortcuts design.
  - New Revamped Volume Panel that adapts to different volume styles.
  - Updated Bootanimation (04/13/24)
  - Updated Seekbar design (04/13/24)
  - Introducing Volume panel sound haptics (04/19/24)
  - Implemented glass blur effect for devices that uses skia render engine (04/19/24)

- **Recovery:**
  - New Revamped user interface.

- **Refresh rate tile:**
  - Added support for devices with unique refresh rates (04/28/24)

- **Settings:**
  - Improved homepage avatar handling; homepage avatar now supports Google account if signed-in, then fallbacks to multi-user redirect if none.
  - Added navigate to multi-user settings on homepage avatar long click if google account is logged-in (04/16/24)
  - Fixed crash when changing monet styles (04/19/24)
  - Fixed UI inconsistencies on some preference sections (04/19/24) 
  - (BUILDING) allowed [overlaying](https://github.com/https://github.com/RisingOS-staging/android_packages_apps_Settings/commit/3299b2665fddc520ef5d71898eaeb51330383d28/). of minimum refresh rate for the new refresh rate picker 
  - Added Hidden SSID, Hotspot client manager and AP band controls changes authored by [cjybyjk](https://github.com/cjybyjk/), forward ported by risingOS team (05/06/24)

- **Settings Styles:**
  - Introducing Settings Styles (RisingUI 2.0/1.0 aka Ayan Card UI).
  - Added Material design settings theme style (04/16/24)
  - Implemented full settings theme integration (04/28/24)

- **Shake Gestures:**
  - Introducing new Shake Gestures feature, shake your device to do stuffs! 
  - Added screenshot option (04/13/24)
  - Improved wakelock handling (04/16/24)

- **Status Bar Chip:**
  - Fixed and improved chip layout (04/28/24)

- **System Fonts:**
  - Improved and optimized font override handling.

- **UDFPS animations/icons:**
  - Added more udfps icons contributed by: Davic Becker, Aditya Choudhury, AnierinB and xpirasians. (04/21/24)
  - Fixed an issue where UDFPS animation gets stucked after unlocking device (05/06/24)

- **Volume Panel:**
  - Minor animations adjustments for slider and dialog panel (04/28/24)

- **WiFi Standard:**
  - Fixed WiFi icon margin when WiFi standard is off/hidden.

---

## 💬 Highlights (Cherry-Picked Additions)

- **UI Styles:**
  - Added user interface styles from Bootleggers by [eldainosor](https://github.com/eldainosor/).

- **New refresh rate selector page:**
  - New refresh rate selector page by [Adithya R](https://github.com/ghostrider-reborn/).

---

## 👴 Deprecated Features (Removed Features)

- **Columbus/Elmyra:**
  - Removed due to deprecated dependencies and will be re-introduced once we learn how to regenerate the new java libraries.

- **LockScreen Album Art Filter:**
  - Deprecated as of [QPR2](https://github.com/crdroidandroid/android_frameworks_base/commit/8f922ec2cb649b99b07a90836584702c4f22e0a9).

- **Nothing Launcher:**
  - Deprecated as of QPR2 update

- **RisingUI Beta QuickSettings:**
  - Removed and will be re-introduced as Quicksettings Styles in upcoming releases.

---

## 🙌 All Features currently shipped with respective Authors and Contributors
Below is a detailed compilation of all features incorporated into the current release, accompanied by the acknowledgments of the original authors and contributors of the listed features.

**Disclaimer:** The risingOS team may have made partial modifications to these features. However, it is essential to note that we do not assert or will NEVER assert ownership to any of these features, nor do we claim any part of them as our own. All copyrights and credits belong to their respective authors and contributors.

Your understanding and appreciation for the creativity and efforts of the original contributors are highly valued. We extend our outmost gratitude and appreciation to all the people listed below for their contributions and efforts to the development of these features 🙏

---
- **LineageOS features and customizations:** LineageOS Project
- **Adaptive Playback:** Jyotiraditya, Stylogey
- **Ai Assistant Shortcut:** Credits to Mishaal Rahman
- **Always on Display schedule:** idoybh
- **Always on Display on Charge:** darkobas, jhonboy121, idoybh, Pranav Vashi (Fixes and Improvements)
- **AppLock:** jhonboy121, Pranav Vashi (Forward Port and fixes)
- **Brightness Slider Customizations:** Alberto97, Michael Bestas, Luca Stefani, Alexander Westphal, qjohn, maxwen, Pranav Vashi, idoybh, timjosten
- **Battery Bar:** cphelps76, Pranav Vashi (Fixes)
- **Battery Customizations:** althafvly, Pranav Vashi, Myself5, TheStrix, ezio84, 703joko, R15Hi, spezi77, StarkDroid, Dr Disagree
- **Colored Status Bar Icons:** Dil3mm4, spkal101, Pranav Vashi (Fixes and Improvements)
- **Disable Data Indicator:** varund7726
- **Edge Light:** jhonboy121, Stallix (Forward Port), Pranav Vashi (Fixes and Improvements)
- **GameSpace:** Nauval Rizky
- **Hide Power Menu on QS:** jhonboy121
- **Island Notification:** Dil3mm4 (author of reticker feature), Pranav Vashi and someone5678 (fixes and improvements)
- **Less Boring Headsup:** ezio84, Rushab Shah, Pranav Vashi
- **Music Ticker:** ezio84, Pranav Vashi (Forward Port)
- **Noisy Notifications:** ezio84
- **Lockscreen Charging Info:** beanstown106
- **LockScreen Clocks:** Afterlife Project (703joko)
- **Lockscreen Media Art:** beanstown106
- **Monet Customizations:** idoybh, Pranav Vashi
- **Notification Count:** Steve Kondik, jhonboy121, Pranav Vashi (Fixes)
- **Omnijaws Weather Client:** Maxwen, Pranav Vashi
- **QuickSettings Tile Animations:** Nico60, PacMM79
- **QuickSettings Header Image:** Idc/ancientOS
- **QuickSettings Styles and Customizations:** IacobIonut01, SamarV-121, Tim Zimmermann, cjh1249131356, timjosten, StarkDroid, Dr Disagree, elluzion, rdx420
- **Screen Off Animations:** Kshitij Gupta, Pranav Vashi (Forward Port),
- **Shape and Icon Pack Themes:** SagarMakhar, Pranav Vashi (Improvements), Dr Disagree (Iconify Icon Packs)
- **Status Bar Clock Customizations:** Luca Stefani, Hendrik Hagendorn, LuK1337, Michael W, Volodymyr Zhdanov, kxxt, bellegarde-c, Pranav Vashi
- **Status Bar Clock Chip:** StarkDroid
- **Status Bar Logo:** Pranav Vashi, Shevt, LorDClockaN, varund7726
- **System Haptics:** Blaster4385, Pranav Vashi, someone5678
- **Smart Pixels:** Sergii Pylypenko, Anay Wadhera, Pranav Vashi, frap129
- **Screenshot Sound:** Ashwin R C
- **Swipe to Screenshot:** ghbhaha, jhenrique09
- **Pulse Visualizer:** bigrushdog (Randall), Pranav Vashi (Forward Port)
- **UDFPS Animations:** SagarMakhar, Dhina17, AnnierinBliss, Pranav Vashi
- **Volume Steps:** Meticulus
- **Volume Styles:** Dr Disagree (iconify volume style packs).

---


