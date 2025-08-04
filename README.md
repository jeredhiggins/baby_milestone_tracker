# Baby Milestone Tracker · Inspired by Mayan Cosmology 🌙

A research-backed developmental milestone tracker built for mobile and offline-first use. Tracks physical, emotional, and cognitive growth from birth to age 5 using a constellation-inspired visual system based on Mayan cosmology.

---

## What It Does

- Over 200 milestones organized by developmental domain
- Each domain is represented with a Mayan-inspired glyph and celestial metaphor
- Cards include:
  - Age range
  - Domain
  - Description
  - Tips
  - Cosmic range (early, average, late bloomers)
- Manual save/load via JSON
- Offline PWA support and Home Screen installable

---

## 📊 Milestone Data Sources

All milestone data was adapted from publicly available scientific and educational sources. Each entry in the milestone file includes a `"source"` field for attribution.

### **Primary Sources**

- **CDC Milestone Checklists (2022 update)**  
  https://www.cdc.gov/ncbddd/actearly/milestones/index.html  
  - Domains: Gross Motor, Fine Motor, Language, Social/Emotional  
  - Referenced via `"source": "CDC"`

- **WHO Motor Development Study**  
  https://www.who.int/tools/motor-development-study  
  - Focus on international motor skills development norms  
  - Referenced via `"source": "WHO"`

- **American Academy of Pediatrics (AAP) – Bright Futures**  
  https://brightfutures.aap.org  
  - Broad developmental categories including self-help and social domains  
  - Referenced via `"source": "AAP"`

- **Zero to Three: Early Development Milestones**  
  https://www.zerotothree.org  
  - Covers cognitive, emotional, and early learning behaviors  
  - Referenced via `"source": "ZeroToThree"`

---

## 📝 Sample Milestone Data

```json
{
  "id": "se_017",
  "title": "Expresses affection with hugs or kisses",
  "domain": "Social-Emotional (Deer / Keh)",
  "age": "12–18 months",
  "description": "Baby shows emotional attachment by initiating hugs or kisses.",
  "tips": "Model and name affectionate behaviors to reinforce them.",
  "range": {
    "average": "14 months",
    "early": "12 months",
    "late": "18 months"
  },
  "source": "ZeroToThree"
}
```

---

## 🌌 Mayan Glyph & Constellation Guide

| Domain              | Glyph Symbol         | Inspiration                    | Meaning                               |
|---------------------|----------------------|---------------------------------|----------------------------------------|
| **Gross Motor**     | 🐆 Jaguar (Balam)     | Mayan protector of the underworld | Strength, balance, mobility            |
| **Fine Motor**      | 🐢 Turtle Shell (Ekʼ) | Symbol of timing, coordination   | Dexterity, manipulation                |
| **Language**        | 🦜 Macaw (Moʼ)         | Known for mimicry and vocal power | Expression, communication              |
| **Cognitive**       | 🦅 Eagle/Vulture (Kʼutz) | High vision, insight          | Memory, reasoning, foresight           |
| **Social-Emotional**| 🦌 Deer (Keh)          | Peaceful & intuitive being       | Bonding, empathy, expression           |
| **Adaptive/Self-Help** | 🌌 Black Road (Xibalba) | Path of trials and growth    | Independence, self-care, transition    |
| **Sensory** (optional) | 🐉 Kukulcán Serpent | Celestial dragon of perception | Balance, sensory integration           |

---

## 💾 Saving and Loading Progress

Progress is stored using `localStorage` and can be manually exported/imported:

### ✅ Save Progress
- Tap **"Save Progress"**
- A file named `baby_milestones_progress.json` is downloaded
- File contains array of completed milestone `id`s

Example:
```json
["gm_001", "lang_005", "cog_007"]
```

### 📥 Load Progress
- Tap **"Load Progress"**
- Choose the saved `.json` file
- Previously completed milestones will be restored and visually updated

---

## 🚀 Deploying the App

- This app is static and compatible with GitHub Pages, Netlify, or [Vercel](https://vercel.com).
- Working Demo: https://baby-milestone-tracker-blush.vercel.app/

### 💡 Quick Start

1. **Fork this repo or clone:**
   ```bash
   git clone https://github.com/yourusername/baby-milestone-tracker.git
   ```

2. **Push to your own GitHub repo**

3. **Deploy with Vercel:**
   - Go to [https://vercel.com](https://vercel.com)
   - Connect your GitHub repo
   - Choose **Static Site**
   - Deploy 🎉
   


---

## 📱 Install as Home Screen App (iOS)

1. Open your deployed app in **Safari**
2. Tap **Share** → “Add to Home Screen”
3. The app icon will appear on your iPhone/iPad with full-screen support

## 🤝 Contributing

Suggestions for improvement or new milestone data are welcome!

- Submit a GitHub issue
- Or send a pull request with:
  - new milestone data (include `"source"` field)
  - updated glyph art
  - additional translations/localizations

---

## 🧠 Credits

- Data: [CDC](https://cdc.gov), [WHO](https://who.int), [AAP](https://aap.org), [Zero to Three](https://zerotothree.org)
- Glyph Art: Custom digital renderings based on authentic Mayan symbolism
- Created with ❤️ by Jered Higgins

---

## 📫 Contact

Want to contribute or collaborate?
🔗 [github.com/jeredhiggins](https://github.com/jeredhiggins)
