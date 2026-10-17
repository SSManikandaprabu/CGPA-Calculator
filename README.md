[README (1).md](https://github.com/user-attachments/files/33601190/README.1.md)
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=220&color=gradient&customColorList=6,2,18&text=Gradeline&fontSize=64&fontColor=ffffff&animation=fadeIn&desc=Tap%20grades.%20Watch%20your%20CGPA%20move.&descSize=20&descAlignY=72" alt="Gradeline banner" />

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-2743FF?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Dependencies](https://img.shields.io/badge/Dependencies-0-0FB57E?style=for-the-badge)
![Dark Mode](https://img.shields.io/badge/Dark_Mode-Supported-7D90FF?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-FFB020?style=for-the-badge)

### 🎓 A fast, beautiful CGPA calculator with a built-in target planner.

[**🌐 Live Demo**](https://YOUR-USERNAME.github.io/gradeline) · [**🐛 Report a Bug**](../../issues) · [**✨ Request a Feature**](../../issues)

</div>

---

## 🎯 Why Gradeline?

Most CGPA calculators are slow forms full of dropdowns. Gradeline replaces them with **one-tap grade chips**, so you can fill a whole semester in seconds. Your CGPA, SGPA and grade mix update live, and the **target planner** tells you what average you need to hit your goal.

## ✨ Features

| | Feature | Details |
|---|---|---|
| 👆 | **One-tap grades** | Colour-coded chips for O, A+, A, B+, B, C and F |
| 📊 | **Live CGPA** | Big, animated-feel readout that recalculates on every change |
| 🧮 | **Per-semester SGPA** | Each semester shows its own score |
| 🌈 | **Grade mix bar** | See your credits split across grades at a glance |
| 🎯 | **Target planner** | Enter a target CGPA and the credits left, and get the average grade needed |
| ➕ | **Flexible structure** | Add or remove semesters and courses freely |
| 💾 | **Auto-save** | Data stays in your browser via `localStorage` |
| 🌗 | **Light and dark themes** | Follows your system, with a manual toggle |
| 📱 | **Responsive** | Sticky summary panel on desktop, stacked layout on mobile |
| ♿ | **Accessible** | Labelled inputs, grouped grade buttons, visible focus rings |

## 🧠 How It Works

Gradeline uses the common **10-point grading scale**:

| Grade | O | A+ | A | B+ | B | C | F |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| **Points** | 10 | 9 | 8 | 7 | 6 | 5 | 0 |

```text
SGPA = Σ (credits × grade points) ÷ Σ credits          (per semester)
CGPA = Σ (credits × grade points) ÷ Σ credits          (across all semesters)
Approx. percentage = CGPA × 10
```

**Target planner**

```text
Required average = (Target × (Credits so far + Credits left) − Points so far) ÷ Credits left
```

It also handles edge cases: if the result is above 10 it tells you the target is not reachable, and if you would clear it even with all F grades it tells you that too.

## 🛠️ Tech Stack

- 🧱 **HTML5** with semantic markup
- 🎨 **CSS3** using custom properties, grid and a system-aware dark mode
- ⚡ **Vanilla JavaScript**: no frameworks, no build step
- 🔤 **Google Fonts**: Bricolage Grotesque and Figtree

## 🚀 Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/YOUR-USERNAME/gradeline.git

# 2. Open the folder
cd gradeline

# 3. Run it (any one of these)
open index.html        # macOS
start index.html       # Windows
npx serve .            # local server
```

No installs and no build step. Just open `index.html`.

## 🎨 Customize

**Change the grading scale** (for example, if your university uses different points):

```js
const G = [["O",10,"--g-O"],["A+",9,"--g-Ap"],["A",8,"--g-A"],["B+",7,"--g-Bp"],["B",6,"--g-B"],["C",5,"--g-C"],["F",0,"--g-F"]];
```

**Change the default credits per course** (currently 4):

```js
const mk = () => ({ n: "", cr: 4, g: "O" });
```

**Change the brand colour** in the `:root` block:

```css
--brand: #2743ff;
```

## 📁 Project Structure

```text
gradeline/
├── index.html    # markup, styles and logic in one file
└── README.md
```

## 🌍 Deploy for Free

| Platform | Steps |
|---|---|
| 🐙 **GitHub Pages** | Settings → Pages → Deploy from branch → `main` |
| ▲ **Vercel** | Import the repo and deploy |
| 🟢 **Netlify** | Drag and drop the folder |

## 🔒 Privacy

Everything runs in your browser. Your grades are saved only in your own `localStorage` and are never sent anywhere.

## 🗺️ Roadmap

- [x] Multi-semester CGPA and per-semester SGPA
- [x] Colour-coded grade mix
- [x] Target CGPA planner
- [x] Light and dark themes
- [ ] Export results as PDF or image
- [ ] Import and export data as JSON
- [ ] Custom grading scales from the UI
- [ ] Shareable result link

## 🤝 Contributing

Contributions are welcome.

1. 🍴 Fork the project
2. 🌿 Create your branch: `git checkout -b feature/amazing-idea`
3. 💾 Commit your changes: `git commit -m "Add amazing idea"`
4. 🚀 Push the branch: `git push origin feature/amazing-idea`
5. 🔁 Open a Pull Request

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for details.

## 👨‍💻 Author

**S.S. Manikanda Prabu**
B.Tech CSE, SRM Institute of Science and Technology, Ramapuram

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/YOUR-USERNAME)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-PROFILE)

<div align="center">

⭐ **If Gradeline helped you, give it a star.** ⭐

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&color=gradient&customColorList=6,2,18&section=footer" alt="footer wave" />

</div>
