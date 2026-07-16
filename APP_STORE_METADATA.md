# Qiyam — App Store Connect Metadata

Everything ready to paste into App Store Connect. Character limits noted per field.

---

## Name
*(max 30 chars)*

```
Qiyam
```

---

## Subtitle
*(max 30 chars — appears under the app name on the product page)*

**English:**
```
Nightly Quran & Qiyam al-Layl
```
*(28 characters)*

English alternatives:
- `Quran Reading Plans & Mushaf` (28)
- `Read the Quran Every Night` (26)
- `Quran, Prayer Times & Qibla` (27)

**Arabic** *(for the `ar` App Store localization):*
```
قيام الليل وقراءة القرآن
```
*(24 characters — "Night prayer and Quran reading")*

Arabic alternatives:
- `اقرأ القرآن كل ليلة` (19) — Read the Quran every night
- `وردك الليلي مع القرآن` (21) — Your nightly portion with the Quran
- `المصحف ومواقيت الصلاة والقبلة` (28) — Mushaf, prayer times & Qibla
- `ختمة القرآن ومواقيت الصلاة` (26) — Quran khatmah & prayer times

---

## Promotional Text
*(max 170 chars — editable anytime without resubmitting the app)*

```
Build a lasting habit of Qiyam al-Layl. Nightly Quran reading plans, an authentic Mushaf, prayer times, and streaks — all in one calm, distraction-free app.
```
*(150 characters)*

---

## Keywords
*(max 100 chars, comma-separated, no spaces after commas. Do NOT repeat the app name — Apple already indexes it.)*

```
quran,mushaf,tahajjud,islam,muslim,prayer,salah,tafsir,khatmah,recitation,qibla,hifz,dua,adhan,surah
```
*(99 characters)*

---

## Description
*(max 4000 chars)*

```
Qiyam — Read the Quran Every Night

Qiyam helps you build and keep a nightly habit of standing with the Quran. Set a reading plan, follow it page by page in a beautiful authentic Mushaf, and watch your streak grow — from the first ayah to a complete Khatmah.

NIGHTLY READING PLANS
• Complete the Quran (Khatmah) in a number of nights you choose
• Read a fixed amount each night — 100 ayat, a set number of pages, or a custom pace
• Fajr-aware reminders so you never miss your night portion
• Reschedule on the fly when life gets busy — the plan adjusts with you

AN AUTHENTIC MUSHAF
• Uthmanic script (QCF) rendered page by page, faithful to the printed Mushaf — all 604 pages
• Optional Tajweed coloring to guide your recitation
• Light, dark, and gentle night-reading modes for comfortable late-night reading
• Pinch to zoom, smooth page turning, and a distraction-free reading chrome

PRAYER TIMES & QIBLA
• Accurate prayer times for your location with a live Fajr countdown
• Built-in Qibla compass to find the direction of prayer anywhere

LISTEN & LEARN
• Ayah-by-ayah audio recitation from multiple reciters
• Word-by-word display to follow along and understand
• Inline tafsir for every ayah, right where you're reading
• Browse the Quran by topic and jump to related verses

TRACK YOUR PROGRESS
• Surah checklist and Khatmah history
• Day-streak tracking to keep your momentum
• Bookmarks with tags to save and organize meaningful verses

REVISION (MURAJA'A)
• Plan and track revision of what you've memorized
• A visual overview of your Quran journey to keep your hifz strong

WORKS OFFLINE
• Download reciters, word-by-word data, and reading packs for offline use
• Read and listen anywhere, no connection needed

Whether you're beginning your first night of Qiyam or completing your next Khatmah, Qiyam is built to keep you close to the Book of Allah — every single night.

We'd love your feedback and du'a. May Allah accept from us and from you.
```

---

## URLs
*(Live on GitHub Pages. Type them by hand into App Store Connect — pasting can insert an invisible character that trips ASC's "URL is formatted incorrectly" validator. Use the no-trailing-slash form.)*

**English (en) localization:**

| Field | URL |
|---|---|
| **Marketing URL** | `https://mohamedsamy25.github.io/qiyam-site` |
| **Support URL** | `https://mohamedsamy25.github.io/qiyam-site/support.html` |
| **Privacy Policy** | `https://mohamedsamy25.github.io/qiyam-site/privacy.html` |

**Arabic (ar) localization:**

| Field | URL |
|---|---|
| **Marketing URL** | `https://mohamedsamy25.github.io/qiyam-site/ar.html` |
| **Support URL** | `https://mohamedsamy25.github.io/qiyam-site/support-ar.html` |
| **Privacy Policy** | `https://mohamedsamy25.github.io/qiyam-site/privacy-ar.html` |

Every page has an **English / العربية** switcher, so either URL leads to both languages.

**If ASC rejects a URL as "formatted incorrectly":**
1. Clear the field completely.
2. Type the URL by hand (don't paste).
3. Omit the trailing slash.
4. Tab out — the error should clear.
5. Still failing? Paste into TextEdit (Format → Make Plain Text) first, then copy from there.

---

## App Privacy (questionnaire — separate from the Privacy Policy URL)

Select **"Data Not Collected."**

Verified from the codebase:
- **No accounts, no analytics, no ads, no tracking SDKs.**
- **Location** is used only on-device for prayer times + Qibla — never transmitted.
- **Network** traffic is only content downloads (audio from mp3quran.net, word-by-word from qurancdn.com, fonts from Cloudflare R2) — no user data sent.
- Content downloads touching third-party CDNs do NOT count as *you* collecting data.

---

## Location Permission String (already set in project.yml)

`NSLocationWhenInUseUsageDescription`:
```
Qiyam uses your location to calculate accurate prayer times and the Qibla direction for your area. Your location stays on your device and is never shared.
```
Regenerated into project.pbxproj via `xcodegen generate` (Debug + Release).

---

## Still To Do (your side, in App Store Connect)

- [ ] Paste the metadata above (Name, Subtitle, Promotional Text, Keywords, Description).
- [ ] Enter the 3 URLs (type by hand).
- [ ] App Privacy → **Data Not Collected**.
- [ ] Upload screenshots — required: 6.9" iPhone; 6.5" recommended.
- [ ] Upload 1024×1024 app icon (`icon_blue.png`).
- [ ] Commit the `project.yml` location-string change to your app branch before archiving.
