# Typly ⌨️✨
**Modern, Fast, Privacy-First Android Keyboard**

Typly is a feature-rich, high-performance, and privacy-respecting custom keyboard application built natively for Android using Jetpack Compose and Kotlin coroutines. Designed from the ground up to offer a seamless typing experience, Typly combines lightning-fast prediction, comprehensive layout customization, and strict privacy guarantees.

---

## 🚀 Key Features

### 1. Advanced Prediction & Autocorrect Engine
- **Asset-Based Dictionary**: Powered by an embedded frequency vocabulary (`dictionary_freq.txt`) loaded into an optimized Trie structure.
- **Bigram Next-Word Prediction**: Predicts subsequent words intelligently based on typing context.
- **Smart Autocorrect**: Safe autocorrect safeguards with frequency-threshold learning.
- **QWERTY Spatial Swipe Typing**: Supports spatial gesture recognition across QWERTY keys.

### 2. Rich Emoji Panel
- **Categorized Emoji Picker**: Dedicated emoji panel featuring 7 major categories (Smileys, People, Animals, Food, Travel, Objects, Flags) with Samsung and iOS styled emojis.
- **Instant Insertion**: Single-tap emoji insertion directly into any input field.

### 3. Layouts & Customization
- **Top Number Row Toggle**: Optional dedicated `0–9` number row toggle in settings.
- **Dedicated Numeric & Phone Keypads**: Automatically switches to a calculator-style numeric or phone layout when number/phone input types are focused.
- **Long-Press Accent Popups**: Holding down character keys (`a`, `e`, `i`, `o`, `u`, `c`, `n`, `s`, `z`) reveals a floating accent selector (`à`, `á`, `â`, `ç`, `ñ`, etc.).
- **Text Shortcuts / Expansion**: Automatic expansion for common abbreviations (`omw` → *"On my way!"*, `brb` → *"Be right back"*, `ty` → *"Thank you"*, `hw` → *"Hello world!"*, etc.).
- **Custom Backgrounds**: Integrated with the Android Photo Picker to set custom keyboard wallpapers.

### 4. Clipboard History & Sensitive Data Protection
- **Persistent Clipboard**: Stores recent text and image clips locally.
- **Sensitive Data Detection**: Automatically detects OTPs, PINs, auth codes, and sensitive clipboard items (`EXTRA_IS_SENSITIVE`).
- **Secure Auto-Clear**: Transiently holds sensitive clips in memory with an automatic timeout and clears the system primary clip safely without wiping unrelated items.
- **Zero Disk Persistence for Sensitive Clips**: Sensitive clips are never written to disk storage.

### 5. Privacy-First Architecture
- **Zero Network/Audio Permissions**: Completely removed `INTERNET`, `VIBRATE`, and `RECORD_AUDIO` permissions. Typly operates 100% offline with zero cloud telemetry or voice listening.
- **Incognito Support**: Automatically honors `EditorInfo.IME_FLAG_NO_PERSONALIZED_LEARNING` to bypass learning in private/incognito fields.
- **Cloud Backup Exclusion**: Configured with backup and data extraction rules to exclude sensitive user dictionaries and clipboard data from cloud backups and device transfers.

### 6. Accessibility & Theme Contrast
- **Theme Contrast Warning**: Real-time WCAG contrast ratio calculation in the custom color editor warns users (`⚠️ Low contrast warning`) if text and key background combinations have poor readability.
- **TalkBack & Touch Targets**: Fully accessible with TalkBack content descriptions and comfortable minimum touch target sizes.

### 7. Performance & Optimization
- **R8 Minification & Resource Shrinking**: Fully optimized with `isMinifyEnabled = true` and `isShrinkResources = true` for a lean APK footprint.
- **Low-End Device Optimization**: Minimized recompositions and allocations using `remember` and `derivedStateOf` for zero per-key typing lag.

---

## 👤 Creator

Typly was architected and developed by **Arijit Saha**
