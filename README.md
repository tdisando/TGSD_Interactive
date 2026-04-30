# Interactive Total Grain Size Distribution (TGSD)

Exploring distribution curves for characterising pyroclastic deposits

---

## About the Model

### Inspiration

This tool is grounded in classic work on decay processes, rare‑event statistics, and fragmentation:

- **Rutherford & Soddy (1902)** — Introduced the concept of exponential decay and memoryless natural processes.  
  https://doi.org/10.1080/14786440209462856

- **Poisson (1837)** — Established the statistical framework for sequences of rare, independent events.

- **Turcotte (1986)** — Applied rare‑event reasoning to brittle failure, showing that crustal fragmentation produces fractal (power‑law) size distributions.  
  https://doi.org/10.1029/JB091iB02p01921

- **Kaminski & Jaupart (1998)** — Demonstrated that explosive magma fragmentation yields characteristic exponential‑type pyroclast size distributions.  
  https://doi.org/10.1029/98JB02795

- **Rosin & Rammler (1933)** — Developed an exponential‑based particle‑size law widely used for ground materials and later adopted in volcanology.  
  https://doi.org/10.1007/BF01439773

- **Weibull (1939)** — Generalized exponential models to describe material strength and age‑dependent failure, forming the modern Weibull distribution.  
  https://doi.org/10.1115/1.4010337

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
| **Weibull / Rosin-Rammler** | $$f(\phi) = \frac{k}{\lambda}\left(\frac{\phi}{\lambda}\right)^{k-1}\exp\left[-\left(\frac{\phi}{\lambda}\right)^{k}\right]$$ | $k$ = shape parameter (control sorting); $\lambda$ = scale parameter (control decay) |

---

## License

MIT License — see [LICENSE](LICENSE) file for details. Free to use, modify, and distribute with attribution.

---

## Contact

**Author:** [tdisando](https://github.com/tdisando)  
**Questions?** [Open an issue](https://github.com/tdisando/TGSD_Interactive/issues)

---

*Made with ❤️ for the volcanology community*
