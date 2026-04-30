# Interactive Total Grain Size Distribution (TGSD)

Exploring distribution curves for characterising pyroclastic deposits

---

## 📖 Table of Contents

- [About the Model](#about-the-model)
- [Distribution Models](#distribution-models)
- [Quick Start](#quick-start)
- [How to Use](#how-to-use)
- [Features](#features)
- [Technical Details](#technical-details)
- [Repository Structure](#repository-structure)
- [Contributing](#contributing)
- [Citation](#citation)
- [License](#license)
- [Contact](#contact)

---

## About the Model

### Research Inspiration

This tool is inspired by fundamental studies in:
- **Radioactive decay** from Rutherford and Soddy (1902; [DOI: 10.1080/14786440209462856](https://doi.org/10.1080/14786440209462856))
- **Sequence of random events** from Poisson (1837)

### Research Questions

This interactive tool explores:
- **Deposit-based distributions of tephras** in natural cases
- **Breakage probability per size step** during fragmentation
- **An approach to magma fragmentation** without atmospheric disturbances

### Scope

The TGSD model characterizes pyroclastic deposits by exploring how grain size distributions relate to eruption style, fragmentation mechanisms, and transport/deposition processes.

---

## Distribution Models

| Distribution | Parameters | Ideal Eruption Style | Key Diagnostic |
|---|---|---|---|
| **Exponential** | λ (rate) | Near-vent Plinian, data-poor | Strictly monotonic log-linear decay |
| **Power Law I** | α, x_min | Fractal fragmentation (phreatomagmatic, Plinian) | Linear log-log plot |
| **Power Law II** | α, x_min, x_max | Same as Power Law I, but with observable limits | Log-log linear + roll-off at tails |
| **Weibull / Rosin–Rammler** | k (shape), λ (scale) | Most eruption types; most versatile | Unimodal or skewed; k controls shape |

### Mathematical Formulations

| Distribution | Equation | Parameters |
|---|---|---|
| **Exponential** | $$f(\phi) = \lambda \, e^{-\lambda (\phi - \phi_0)}$$ | $\lambda$ = rate parameter (steepness of decay); $\phi_0$ = coarsest grain size (onset phi) |
| **Power Law I** | $$f(\phi) = \frac{\alpha-1}{\phi_{\min}}\left(\frac{\phi}{\phi_{\min}}\right)^{-\alpha}$$ | $\alpha$ = power-law exponent (fractal slope in log-log); $\phi_{\min}$ = lower bound |
| **Power Law II** | $$f(\phi) = \frac{1-\alpha}{\phi_{\max}^{1-\alpha}-\phi_{\min}^{1-\alpha}}\,\phi^{-\alpha}$$ | $\alpha$ = fractal exponent; $\phi_{\min}$ = coarse cutoff; $\phi_{\max}$ = fine cutoff |
| **Weibull / Rosin-Rammler** | $$f(\phi) = \frac{k}{\lambda}\left(\frac{\phi}{\lambda}\right)^{k-1}\exp\!\left[-\left(\frac{\phi}{\lambda}\right)^{k}\right]$$ | $k$ = shape parameter (controls sorting); $\lambda$ = scale parameter |

---

## Quick Start

### 🌐 Try It Online

The interactive tool is hosted on GitHub Pages:

👉 **[https://tdisando.github.io/TGSD_Interactive/](https://tdisando.github.io/TGSD_Interactive/)**

### 💻 Local Setup

1. Clone: `git clone https://github.com/tdisando/TGSD_Interactive.git`
2. Open `index.html` in your browser
3. Or use: `python -m http.server 8000` and navigate to `http://localhost:8000`

---

## How to Use

1. **Select Distribution Model** from the dropdown menu
2. **Adjust Parameters** using sliders—real-time updates show distribution changes
3. **Interpret Plots**: Left plot (linear scale), Right plot (log-log scale)
4. **Analyze**: Compare predictions with your pyroclastic deposit data

---

## Features

✨ Interactive visualization with real-time parameter adjustment  
🔬 Scientifically rigorous distribution models  
📊 Four distribution models (Exponential, Power Law I/II, Weibull)  
🎯 Eruption style interpretation guidance

---

## Technical Details

**Browser Compatibility:** Chrome, Firefox, Safari, Edge (latest versions)  
**Dependencies:** Pure HTML5 + JavaScript (no external libraries)  
**File Size:** ~17 KB  
**Performance:** Works offline once loaded

---

## Repository Structure

```
TGSD_Interactive/
├── index.html          # Main interactive tool
├── README.md           # Documentation
├── LICENSE             # MIT License
```

---

## Contributing

We welcome contributions! Found a bug? Have a feature idea? [Open an issue](https://github.com/tdisando/TGSD_Interactive/issues) or submit a Pull Request.

---

## Citation

If you use this tool in your research, please cite:

**BibTeX:**
```bibtex
@software{tdisando2026tgsd,
  author = {Disando, T.},
  title = {Interactive Total Grain Size Distribution (TGSD)},
  year = {2026},
  url = {https://github.com/tdisando/TGSD_Interactive}
}
```

**APA:**
Disando, T. (2026). Interactive Total Grain Size Distribution (TGSD). GitHub. https://github.com/tdisando/TGSD_Interactive

---

## License

MIT License — see [LICENSE](LICENSE) file for details. Free to use, modify, and distribute with attribution.

---

## Contact

**Author:** [tdisando](https://github.com/tdisando)  
**Questions?** [Open an issue](https://github.com/tdisando/TGSD_Interactive/issues)

---

*Made with ❤️ for the volcanology community*