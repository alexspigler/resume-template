# resume-template

A clean, modern, and highly customizable LaTeX resume template built for precision formatting, easy tuning, and ATS compatibility.

Based on: https://github.com/jakegut/resume (Jake Gutierrez)  
Which itself was based on: https://github.com/sb2nov/resume (Sourabh Bajaj)

---

## Quick Start

1. Install a LaTeX distribution ([MacTeX](https://www.tug.org/mactex/), [MiKTeX](https://miktex.org/), or [TeX Live](https://www.tug.org/texlive/))

2. Edit `resume-template.tex` with your information

3. Compile:
```bash
pdflatex resume-template.tex
```

---

## What's Different?

This version extends Jake Gutierrez’s original template with several key improvements:

- **Fine-grained spacing control** - separate tuning for line spacing within bullets (`baselineskip`) and spacing between bullets (`arraystretch`) for better layout precision.
- **Modular section configuration** - Each section (Education, Experience, Projects, Skills) can be independently tuned or reordered without breaking formatting. All layout logic is self-contained, making it easy to disable, duplicate, or restyle sections.
- **Centralized configuration** - all customization parameters are collected at the top of the file in clearly labeled sections for quick access.
- **Refactored structure for maintainability** - Redundant commands were consolidated, comments standardized, and indentation normalized for easier reading, editing, and version control.

## Preview

![Resume Template](resume-template.png)

---