# resume-template

A clean, modern, and highly customizable LaTeX resume template built for precision formatting, easy tuning, and ATS compatibility.

Based on: https://github.com/jakegut/resume (Jake Gutierrez)  
Which itself was based on: https://github.com/sb2nov/resume (Sourabh Bajaj)

---

## Features

- **Independent spacing controls** - separate parameters for space between bullets and within wrapped lines, plus indentation and margin settings
- **Centralized customization** - all parameters clearly grouped and documented (no digging through code)
- **ATS-friendly design** - fully machine-readable and optimized for applicant tracking systems
- **Flexible typography** - quickly switch between multiple sans-serif and serif fonts

## Quick Start

1. Install a LaTeX distribution ([MacTeX](https://www.tug.org/mactex/), [MiKTeX](https://miktex.org/), or [TeX Live](https://www.tug.org/texlive/))

2. Edit `resume-template.tex` with your information

3. Compile:
```bash
pdflatex resume-template.tex
```

## Customization

All section-specific spacing and indentation settings are defined near the top of the file under “Tunable Settings.”

**Example - adjust bullet spacing in the "Project" section:**
```latex
\newcommand{\ProjBulHeight}{\renewcommand{\arraystretch}{1.25}}  % space between bullets
\newlength{\ProjWrapHeight} \setlength{\ProjWrapHeight}{11pt}    % space within wrapped lines
```

Increase the first for more space between bullets, or decrease the second to tighten wrapped lines under the same bullet.

Each section (Education, Experience, Projects, Skills) has its own labeled control block — just search for the comments.

## What's Different?

This version extends Jake Gutierrez’s original template with several key improvements:

- **Fine-grained spacing control** - separate tuning for line spacing within bullets (`baselineskip`) and spacing between bullets (`arraystretch`) for better layout precision.
- **Modular section configuration** - Each section (Education, Experience, Projects, Skills) can be independently tuned or reordered without breaking formatting. All layout logic is self-contained, making it easy to disable, duplicate, or restyle sections.
- **Centralized configuration** - all customization parameters are collected at the top of the file in clearly labeled sections for quick access.
- **Refactored structure for maintainability** - Redundant commands were consolidated, comments standardized, and indentation normalized for easier reading, editing, and version control.

## Preview

![Resume Template](resume-template.png)

---