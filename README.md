# Vedic Scriptures Crowdsourcing Database

Welcome to the crowdsourced data repository for the Vedic Scholar platform. This repository hosts structured, version-controlled Markdown files containing the Vedas and Upanishads. 

Our goal is to leverage the open-source community to crowdsource, verify, and preserve authentic Sanskrit Devanagari texts, IAST transliterations, and English translations of these ancient scriptures.

---

## 📁 Repository Structure

To make crowdsourcing simple and avoid Git merge conflicts, the scriptures are organized into modular, self-contained files:

```text
├── rigveda/
│   ├── mandala_01/
│   │   ├── hymn_001.md
│   │   ├── hymn_002.md
│   │   └── ...
│   ├── mandala_02/
│   └── ... (Mandalas 01 to 10)
└── upanishads/
    ├── isha_upanishad.md
    ├── katha_upanishad.md
    ├── kena_upanishad.md
    └── mundaka_upanishad.md
```

- **Rigveda**: Organized by Mandala (Books 1-10) and subdivided into individual hymns/suktas (`hymn_xxx.md`).
- **Upanishads**: Organized as individual files per Upanishad due to their shorter lengths.

---

## 📝 Markdown File Schema

Each scripture file follows a strict frontmatter and heading hierarchy to allow the platform's Full-Text Search (FTS5) engine to index it automatically:

```markdown
---
title: "Rigveda Mandala 1, Hymn 1"
category: "Rigveda"
chapter: "Mandala 1"
hymn: "Hymn 1"
---

# Verse 1

## Sanskrit
अ॒ग्निमी॑ळे पु॒रोहि॑तं य॒ज्ञस्य॑ दे॒वमृ॒त्विज॑म् ।
होता॑रं रत्न॒धात॑मम् ॥ १ ॥

## IAST
agnimīḷe purohitaṃ yajñasya devamṛtvijam |
hotāraṃ ratnadhātamam || 1 ||

## Translation
I praise Agni, the chosen Priest, the God, the Minister of sacrifice, the Hotar, lavisher of wealth.

---
```

---

## 🤝 How to Contribute

We welcome contributions of all sizes! Whether you are correcting a typo in an English translation, adding original Sanskrit Devanagari text, or providing IAST transliterated verses, here is how you can help:

### Contributing via Pull Request (GitHub)
1. **Fork** this repository to your own account.
2. **Clone** your fork locally.
3. Locate the specific file you want to edit (e.g. `rigveda/mandala_01/hymn_001.md`).
4. Replace placeholder brackets like `[Add Devanagari Sanskrit]` or `[Add IAST Transliteration]` with the authentic text.
5. **Commit** your changes with a clear message:
   ```bash
   git commit -am "Add Sanskrit text for Rigveda 1.1.1-1.1.5"
   ```
6. **Push** your changes to your fork and submit a **Pull Request** to this main repository.

### Rules of Thumb
- **Devanagari Sanskrit**: Ensure Unicode characters are entered correctly with proper Vedic accents if available.
- **IAST Transliteration**: Use standard International Alphabet of Sanskrit Transliteration diacritics (e.g., `ā`, `ī`, `ū`, `ṛ`, `ṣ`, `ṭ`, `ḍ`, `ṇ`, `ṃ`, `ḥ`).
- **Translations**: Cite the translator in your commit message if importing new public domain translations.
