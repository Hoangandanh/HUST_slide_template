# 🎓 HUST Beamer Template for LaTeX Presentations

A **professional, flexible, and modern Beamer theme** designed for academic and research presentations at **Hanoi University of Science and Technology (HUST)**.  
This template focuses on **visual consistency, simplicity, and customization**, helping lecturers, students, and researchers create polished and institution-branded slide decks directly in **LaTeX**.

---

## 🌟 Key Features

### 🏫 Professional HUST Branding
- Official **HUST color palette** (`HUSTRed`, `HUSTBlue`) for a cohesive academic look.  
- Multiple **logo variants** (with/without text, bilingual versions) adjustable by package options.  
- Consistent **footer layout** with logo placement and red signature bar, rendered precisely via TikZ.

### 🎨 Flexible and Customizable Design
- Support for **theme colors**: `blue` or `red`, easily switched via options.  
- Automatic or manual **aspect ratio detection** (`auto`, `169`, or `43`).  
- Control over **backgrounds, logos, and branding slides** through simple commands:
  ```latex
  \HUSTUseBackground{theme.pdf}
  \HUSTInsertBrandSlide
  \HUSTInsertThemeSlide
  \HUSTClearBackground
  ```
- Dynamically computed **logo scaling** based on original pixel dimensions — ensuring proportional rendering on all screen sizes.


---

## 🧰 Options Overview

| Option         | Default | Description |
|----------------|----------|-------------|
| `theme`        | `blue`   | Choose between `blue` or `red` color scheme |
| `aspectratio`  | `auto`   | Detect from Beamer (`169` or `43`), or specify manually |
| `logo`         | `logo`   | Select logo variant (`logo`, `logowithtext`, `hust`, `hustwithtext`, etc.) |

---

## 🧱 Commands Reference

| Command | Purpose |
|----------|----------|
| `\HUSTUseBackground{file}` | Set background for current and following slides |
| `\HUSTUseBackgroundOpt[options]{file}` | Add background with custom scaling |
| `\HUSTClearBackground` | Remove background for subsequent slides |
| `\HUSTInsertBrandSlide` | Insert full-page branded cover slide |
| `\HUSTInsertThemeSlide` | Insert themed divider slide |
| `\HUSTCornerImage[height][x][y]{file}` | Place corner image (e.g., decorative logo) |

---

## 🧑‍💻 Example Usage

```latex
\documentclass[aspectratio=169]{beamer}
\usetheme[theme=blue,logo=logowithtexten]{HUST}

\title{Introduction to Data Structures}
\author{Dr. Nguyen Van A}
\institute{Hanoi University of Science and Technology}
\date{\today}

\begin{document}

\HUSTInsertBrandSlide
\HUSTInsertThemeSlide

\begin{frame}{Overview}
  \begin{itemize}
    \item Professional and consistent academic styling
    \item Automated logo and bar positioning
    \item Full control over color and layout
  \end{itemize}
\end{frame}

\HUSTInsertOnesideSlide

\end{document}
```

---

## 💡 Why Use This Template?

- 📚 **Designed for academia:** Perfect for HUST lectures, theses, and research defense slides.  
- ⚙️ **Fully automated:** No manual alignment or pixel tweaking needed.  
- 🎨 **Highly customizable:** Change color themes, logos, and slide ratios effortlessly.  
- 🧾 **Consistent and modern:** Ensures every presentation reflects HUST’s identity while maintaining Beamer’s professional quality.  

---

## 🏁 License & Credits

© 2025 Hanoi University of Science and Technology.  
This template was developed to promote professional academic presentation standards using open-source LaTeX.  
You may reuse and adapt it under the **LaTeX Project Public License (LPPL)** with attribution.

---

### ✨ Maintainer
**HUST School of Information and Communication Technology (SoICT)**  
Contributors: Dr. Nguyen Quoc Tuan