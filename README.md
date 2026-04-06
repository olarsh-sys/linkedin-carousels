# 📊 LinkedIn Carousels — Economics, Finance & Data Science

---

## Carousels

### 01 · Double Machine Learning
> How ML handles confounders so you can estimate causal effects cleanly.

**Topics covered:** Partially linear model, orthogonalisation, nuisance estimation, residual-on-residual regression, cross-fitting.

**Key references:**
- Chernozhukov, V., Chetverikov, D., Demirer, M., Duflo, E., Hansen, C., Newey, W. & Robins, J. (2018). "Double/debiased machine learning for treatment and structural parameters." *The Econometrics Journal*, 21(1), C1–C68.

📁 [`01-double-ml/`](01-double-ml/)

---

### 02 · The Fama–French Factor Model
> Why your fund's alpha might just be exposure to well-known risk factors.

**Topics covered:** CAPM and its limitations, the size premium (SMB), the value premium (HML), the three-factor and five-factor models, alpha decomposition, factor construction methodology, the factor zoo problem, and the decade-by-decade story of value investing.

**Data:** Kenneth French's Data Library (1926–2025) — [mba.tuck.dartmouth.edu](https://mba.tuck.dartmouth.edu/pages/faculty/ken.french/data_library.html)

**Key references:**
- Fama, E. & French, K. (1993). "Common risk factors in the returns on stocks and bonds." *Journal of Financial Economics*, 33(1), 3–56.
- Fama, E. & French, K. (2015). "A five-factor asset pricing model." *Journal of Financial Economics*, 116(1), 1–22.
- Harvey, C., Liu, Y. & Zhu, H. (2016). "…and the cross-section of expected returns." *Review of Financial Studies*, 29(1), 5–68.

📁 [`02-fama-french/`](02-fama-french/)

---

## Repo Structure

```
├── README.md
├── LICENSE
├── 01-double-ml/
│   ├── double_ml_carousel.tex
│   └── double_ml_carousel.pdf
├── 02-fama-french/
│   ├── famafrench_carousel.tex
│   ├── famafrench_carousel.pdf
│   └── famafrench_data.xlsx
```

---

## How to Compile

Each `.tex` file compiles with **pdfLaTeX**. Run twice to resolve bookmarks and cross-references:

```bash
pdflatex carousel.tex
pdflatex carousel.tex
```

**Dependencies:** Standard TeX Live installation with `beamer`, `tikz`, `pgfplots`, `booktabs`, `amsmath`, and `hyperref`. If your distribution includes `lmodern`, add `\usepackage{lmodern}` to the preamble for cleaner font rendering.

---

## How to Use on LinkedIn

1. Compile the `.tex` file to PDF (or use the included PDF directly).
2. Create a new LinkedIn post and select **Document**.
3. Upload the PDF — LinkedIn will convert each page into a swipeable slide.
4. Add your caption and hashtags.

The carousels are designed at **14.4 cm × 18.0 cm** (4:5 ratio), which maps to LinkedIn's recommended 1080 × 1350 px document format.

---

## Design System

All carousels share a consistent visual identity:

| Element | Value |
|---|---|
| Ink (primary text) | `RGB(12, 14, 18)` |
| Accent (blue) | `RGB(27, 100, 209)` |
| Accent orange | `RGB(225, 108, 32)` |
| Accent green | `RGB(33, 158, 115)` |
| Accent purple | `RGB(120, 72, 221)` |
| Muted (secondary text) | `RGB(100, 106, 115)` |
| Soft (backgrounds) | `RGB(245, 247, 250)` |
| Aspect ratio | 4:5 portrait (14.4 × 18.0 cm) |
| Engine | pdfLaTeX + Beamer |

---

## Upcoming

More carousels in progress — potential topics include:

- Regression Discontinuity Design
- Difference-in-Differences
- Instrumental Variables
- Value at Risk vs. Expected Shortfall
- Simpson's Paradox

---

## Author

Muiz Olasupo
