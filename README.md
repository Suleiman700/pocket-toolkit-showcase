<p align="center">
  <img src="assets/icon.png" width="112" alt="Pocket Toolkit icon" />
</p>

<h1 align="center">Pocket Toolkit</h1>

<p align="center">
  <b>76 offline tools in one Android app</b> — level, compass, ruler, flashlight, sound meter, calculators and much more.<br/>
  Built with Expo, React Native and a custom Kotlin native module.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Android-3DDC84?logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Expo_SDK-57-000020?logo=expo&logoColor=white" alt="Expo SDK 57" />
  <img src="https://img.shields.io/badge/React_Native-0.86-61DAFB?logo=react&logoColor=black" alt="React Native 0.86" />
  <img src="https://img.shields.io/badge/Kotlin-native_module-7F52FF?logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/TypeScript-strict-3178C6?logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/languages-EN_·_AR_·_HE_·_ES-F4B63F" alt="Languages" />
</p>

> **Showcase repository.** This is a public preview of a published Android app. **Source code is not included** — only documentation, screenshots and design notes. See [Status & Licensing](#status--licensing) at the bottom.

<p align="center">
  <img src="assets/banner.png" alt="Pocket Toolkit" width="760" />
</p>

---

## Table of Contents

- [Highlights](#highlights)
- [In Motion](#in-motion)
- [Screenshots](#screenshots)
- [All 76 Tools](#all-76-tools)
- [Tech Stack](#tech-stack)
- [Architecture](#architecture)
- [Native Module](#native-module)
- [Engineering Notes](#engineering-notes)
- [Privacy](#privacy)
- [Status & Licensing](#status--licensing)

---

## Highlights

- **76 tools in 8 categories** — measuring, outdoors, light & sound, camera & codes, electronics, calculators, everyday utilities and phone diagnostics.
- **Fully offline.** No account, no sign-up, no server. Every measurement is processed on the device.
- **Real sensors, real hardware** — accelerometer, gyroscope, magnetometer, barometer, light sensor, step counter, GNSS satellites, microphone FFT, camera, flash, NFC, Bluetooth LE and Wi-Fi.
- **Custom Kotlin native module** (≈1.9k lines) for everything Expo doesn't cover: live audio spectrum, GNSS sky view, flash patterns, home-screen widgets, a Quick Settings tile, exact alarms, calendar conversion, lossless photo metadata stripping and more.
- **4 languages including RTL** — English, Arabic, Hebrew and Spanish, with correct plural rules for Arabic (6 forms) and Hebrew (3 forms).
- **Polished motion** — Reanimated 4 springs and layout transitions, drag-to-reorder tool grids, haptics that respect the user's settings.
- **Accessibility and comfort** — light, dark, AMOLED and night-red themes, large "fullscreen reading" mode, orientation-aware tools.
- **Emergency screen** — SOS light, loud siren and one-tap calling of the local emergency number.
- **Home-screen presence** — tools widget, countdown widget, app-icon shortcuts and a flashlight tile in Quick Settings.

---

## In Motion

<table>
  <tr>
    <td align="center"><img src="assets/gifs/tools-home.gif" width="240" alt="Tools home" /><br/><sub><b>Tools home</b><br/>categories, favorites, drag to reorder</sub></td>
    <td align="center"><img src="assets/gifs/bubble-level.gif" width="240" alt="Bubble level" /><br/><sub><b>Bubble level</b><br/>smoothed sensor fusion, turns green when level</sub></td>
    <td align="center"><img src="assets/gifs/stopwatch.gif" width="240" alt="Stopwatch" /><br/><sub><b>Stopwatch</b><br/>laps with fastest / slowest highlighted</sub></td>
  </tr>
</table>

---

## Screenshots

### English

<p>
  <img src="assets/screenshots/en/01_home.png" width="190" />
  <img src="assets/screenshots/en/02_compass.png" width="190" />
  <img src="assets/screenshots/en/03_level.png" width="190" />
  <img src="assets/screenshots/en/04_sunMoon.png" width="190" />
</p>
<p>
  <img src="assets/screenshots/en/05_stopwatch.png" width="190" />
  <img src="assets/screenshots/en/06_resistorCode.png" width="190" />
  <img src="assets/screenshots/en/07_qr.png" width="190" />
  <img src="assets/screenshots/en/08_text.png" width="190" />
</p>

### العربية (RTL)

<p>
  <img src="assets/screenshots/ar/01_home.png" width="190" />
  <img src="assets/screenshots/ar/02_qibla.png" width="190" />
  <img src="assets/screenshots/ar/03_calendars.png" width="190" />
  <img src="assets/screenshots/ar/04_compass.png" width="190" />
</p>
<p>
  <img src="assets/screenshots/ar/05_sunMoon.png" width="190" />
  <img src="assets/screenshots/ar/06_level.png" width="190" />
  <img src="assets/screenshots/ar/07_resistorCode.png" width="190" />
  <img src="assets/screenshots/ar/08_textTools.png" width="190" />
</p>

---

## All 76 Tools

<details open>
<summary><b>📏 Measure (14)</b></summary>

| Tool | What it does |
|---|---|
| Bubble level | Surface and edge modes, switches automatically when the phone is laid flat or stood on an edge |
| Inclinometer | Angle in degrees |
| Ruler | On-screen ruler in cm and inches, calibrated to the real screen density |
| Camera protractor | Measure angles over the camera image |
| Metal detector | Finds magnetic metal with the magnetometer |
| Magnetic field | Field strength on 3 axes |
| Vibration meter | Seismograph-style shaking graph |
| Sound meter | Approximate dB with min and max |
| Light meter | Brightness in lux |
| Height meter | Height of trees and buildings by camera and tilt |
| Distance meter | How far away something is, by camera |
| Camera level | Level and plumb line over the camera |
| Real-size references | Ring sizer, bolts, drill bits and paper at true size |
| Tachometer | Rotation speed in RPM from the gyroscope |

</details>

<details>
<summary><b>🧭 Outdoors (10)</b></summary>

| Tool | What it does |
|---|---|
| Compass | Heading with true north (magnetic declination model) |
| Altimeter | Height from air pressure |
| Speedometer | Speed from GPS |
| Step counter | Steps and distance from the hardware step sensor |
| Sun & moon | Sunrise, sunset, golden hour and moon phase |
| Lightning distance | How far away the storm is |
| Qibla | Direction of the Kaaba with distance |
| GPS distance & area | Walk to measure length or area (m², hectares, dunams, acres) |
| Parking reminder | Find your car again, with a reminder notification |
| GPS status | Satellite sky view, signal bars, accuracy; DD / DMS / UTM / MGRS / Plus Code |

</details>

<details>
<summary><b>🔦 Light & sound (10)</b></summary>

| Tool | What it does |
|---|---|
| Flashlight | Strobe, SOS and Morse patterns |
| Screen light | Bright screen as a light, any color |
| Tone generator | Play any frequency, 20 Hz – 20 kHz |
| Metronome | Keep the beat, with accents |
| Morse translator | Text to Morse and back, with sound and light |
| Voice recorder | Record voice memos, stored privately on the device |
| Sound spectrum | Live FFT analyzer with peak note detection |
| Stroboscope | Freeze spinning things and read their RPM |
| Speaker cleaner | Low-frequency tones to push water and dust out |
| Hearing test | Highest pitch you can hear, per ear |

</details>

<details>
<summary><b>📷 Camera & codes (6)</b></summary>

| Tool | What it does |
|---|---|
| Magnifier | Zoom with noise-reduced captures and reading filters |
| Mirror | Front camera with a light ring |
| Color picker | Identify colors (HEX, RGB, HSL, name) |
| QR scanner | QR codes and barcodes |
| QR & barcode maker | QR for text, links and Wi-Fi; EAN-13, UPC-A, Code 128 |
| Photo metadata | See what a photo reveals and remove its location before sharing (lossless) |

</details>

<details>
<summary><b>🔌 Electronics (3)</b></summary>

| Tool | What it does |
|---|---|
| Resistor color code | Bands to ohms and back (4, 5 and 6 bands) |
| Ohm's law | V, I, R, P and LED resistor calculator |
| Wire gauge | AWG ↔ mm², current rating, real-size cross-section |

</details>

<details>
<summary><b>🧮 Calculators (8)</b></summary>

| Tool | What it does |
|---|---|
| Calculator | Everyday math with % |
| Unit converter | Length, weight, temperature and more |
| Number bases | Decimal, hex, binary, Roman |
| Date calculator | Days between dates, add or subtract days |
| Tip & split | Tip and split the bill |
| Percent & VAT | Percentages, stacked discounts, VAT add / remove, margin vs markup |
| Unit price | Which pack is cheaper per kg or litre |
| Materials calculator | Paint, tiles, flooring and concrete |

</details>

<details>
<summary><b>⏱️ Everyday (13)</b></summary>

| Tool | What it does |
|---|---|
| Timer | Multiple countdowns with alarms that ring even when the app is closed |
| Stopwatch | Laps, fastest / slowest highlighted, fullscreen tap-to-lap |
| Interval timer | Pomodoro, Tabata and HIIT |
| Countdown | Days until your events, with a home-screen widget |
| World clock | Time in other cities |
| Hijri & Hebrew calendar | Convert dates between Gregorian, Hijri and Hebrew |
| Tally counter | Count anything |
| Score keeper | Scores for games and players |
| Random picker | Coin, numbers and lists |
| Password generator | Strong random passwords from a secure source |
| Breathing | Guided calm breathing |
| Text counter | Words, characters, reading time |
| Text & dev tools | Base64 / URL / HTML codecs, MD5–SHA-512 + HMAC, JSON, JWT, UUID / ULID, timestamps, regex |

</details>

<details>
<summary><b>📱 Phone & wireless (12)</b></summary>

| Tool | What it does |
|---|---|
| Device info | Phone, screen and sensors |
| Battery info | Health, temperature, charging speed |
| Storage speed test | Sequential and random read / write |
| Screen tests | Touch, multi-touch, gradients and uniformity |
| Dead pixel test | Full-screen color cycling |
| Sensor dashboard | Every sensor, live |
| Wi-Fi scanner | Nearby networks, channels and signal |
| Bluetooth scanner | Nearby Bluetooth LE devices |
| NFC reader | Read NFC tags and cards |
| Cell signal | Mobile signal in dBm, network type, nearby cells |
| Network info | IP, gateway, DNS, Wi-Fi link |
| Speaker & mic test | Left / right, frequency sweep and mic check |

</details>

---

## Tech Stack

| Layer | Tech |
|---|---|
| **Framework** | Expo SDK 57 · React Native 0.86 (New Architecture) · React 19 |
| **Language** | TypeScript (strict) · Kotlin for the native module |
| **Navigation** | Expo Router (file-based) |
| **Animation & gestures** | Reanimated 4 · Gesture Handler · react-native-sortables (drag to reorder) |
| **Graphics** | react-native-svg (dials, gauges, sky plots, charts) |
| **Storage** | MMKV (settings, favorites, history, backups) |
| **i18n** | i18next with a CLDR plural-rules shim for Hermes · RTL layout |
| **Device APIs** | expo-sensors · expo-camera · expo-audio · expo-location · BLE PLX · NFC manager |
| **Ads & consent** | Google Mobile Ads with Google UMP consent (GDPR / US states) |
| **Build & release** | Continuous Native Generation · custom config plugins · R8 shrinking · Keychain-backed signing script |
| **Tooling** | ESLint (React Compiler rules) · Prettier · tsc strict |

---

## Architecture

```
 app/                         Expo Router screens (tabs, tool/[id], onboarding, emergency, help)
  │
  ├─ Tool registry ───────────  one meta per tool: icon, sensors, permissions, settings schema
  │     │                      → home grid, search index, availability checks, settings UI
  │     ▼
  ├─ ToolShell ───────────────  shared frame for every tool: top bar, hold, save, history,
  │                            share, fullscreen reading, help, calibration prompts
  │
  ├─ Feature modules ─────────  one folder per tool, pure calculation logic kept separate
  │                            from UI so it can be unit-tested (resistor, AWG, UTM/MGRS,
  │                            Plus Code, barcode encoders, codecs, JWT, regex…)
  │
  ├─ Sensor layer ────────────  hooks over expo-sensors + native streams, low-pass /
  │                            time-constant filtering, screen-rotation aware math
  │
  └─ pocket-native (Kotlin) ──  Expo Modules API: functions + event streams for the
                               hardware Expo doesn't expose (see below)
```

- **Registry-driven.** Adding a tool means adding one folder and one meta entry; the home grid, search, categories, availability ("needs a gyroscope"), permissions flow and settings screen pick it up automatically.
- **Permissions only when needed.** Each tool declares its permissions; they're requested the first time that tool opens — never at launch.
- **Offline-first data.** Everything lives in MMKV on the device, with file-based backup and restore.

---

## Native Module

A custom Expo module written in Kotlin (`pocket-native`, ~16 source files):

| Area | What it does |
|---|---|
| **Audio spectrum** | `AudioRecord` at 44.1 kHz, Hann-windowed 4096-point FFT, 96 log-spaced bands streamed to JS |
| **GNSS** | `GnssStatus` satellites (constellation, C/N0, elevation, azimuth, used-in-fix) + raw GPS fixes |
| **Torch** | Flash on/off and precise on/off patterns for strobe, SOS, Morse and the stroboscope |
| **Widgets & tile** | Tools widget, countdown widget and a Quick Settings flashlight tile |
| **Timer alarms** | Exact alarms that ring with the app closed and survive reboots |
| **Calendars** | ICU-based Gregorian ↔ Hijri ↔ Hebrew conversion |
| **Photo metadata** | Private copy via the system photo picker, EXIF read, lossless JPEG / PNG / WebP stripping that keeps rotation and colour profile |
| **Diagnostics** | Battery, storage speed tests, sensor streams, refresh rates, network and cell info, Wi-Fi scan |
| **Text** | Hashes and HMAC, ICU number spell-out in 4 languages |

---

## Engineering Notes

A few problems worth solving properly:

- **Hermes has no `Intl.PluralRules`**, so i18next silently collapsed Arabic and Hebrew to singular/plural. A small CLDR-based shim restores all six Arabic forms and the Hebrew dual.
- **Audio players that keep playing** after `remove()` on Android — every player is now explicitly silenced and paused before it's released.
- **Fast home screen with 76 animated, sortable cards.** Category grids are memoized, stay mounted while searching, and mount progressively after the first frame; search runs against a pre-normalized index (accents, niqqud and Arabic diacritics stripped).
- **Sensor smoothing as a time constant** rather than a per-sample factor, so the level behaves the same at any sensor rate, with a spring-driven bubble that keeps its momentum.
- **Play Store manifest conflicts** from a third-party library's permission declarations, fixed at build time with a config plugin — native folders are never edited by hand.

---

## Privacy

- No accounts, no servers, no analytics of the tools' data. Measurements, photos, recordings and locations stay on the device.
- The only data that leaves the phone is what Google AdMob needs to show ads, behind Google's consent form where the law requires it.
- Full policy: **[brightpixel.work/pages/pocket-toolkit/privacy-policy](https://brightpixel.work/pages/pocket-toolkit/privacy-policy)**

---

## Status & Licensing

**Status:** version 1.0.0 submitted to Google Play.

This repository exists to **showcase** the project. It contains:

- This README
- Screenshots, animated previews and store graphics

It does **not** contain:

- Source code (app, native module, config plugins, scripts)
- Signing keys, ad unit configuration or any credentials
- Design source files

> **© All rights reserved.** All text, images and design content here are the author's. No license is granted: you may not copy, modify, redistribute or use any of this material — including the screenshots — without prior written permission. Viewing on GitHub is fine; everything else is not.

Made by **Suleiman** · [BrightPixel](https://brightpixel.work) · for collaboration or licensing, open an issue or reach out through the website.
