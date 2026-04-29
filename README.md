# TGSD_Interactive
Exploring distribution curves for characterising pyroclastic deposits

## About the models
Inspired by study of radioactive decay from Rutherford and Soddy (1902; https://doi.org/10.1080/14786440209462856) and sequence of random events from Poisson (1837; https://doi.org/10.48550/arXiv.1902.02782), fractal fragmentation theory (pure and truncated Paretos) from Turcotte (1986; https://doi.org/10.1029/JB091iB02p01921) and Kaminski and Jaupart (1992; https://doi.org/10.1029/98JB02795), and  material failure test from Weibull (1939; https://doi.org/10.1115/1.4010337) and crushing coal from Rosin and Rammler (1933; https://doi.org/10.1007/BF01439773).


Trying to understand:
- Deposit-based distributions of tephras in natural cases
- Breakage probability per size step
- An approach to magma fragmentation, yet ideally without atmospheric disturbances

  

| Distribution            | Parameters                 | Ideal eruption style                               | Key diagnostic                                   |
|-------------------------|-----------------------------|-----------------------------------------------------|--------------------------------------------------|
| **Exponential**         | λ (rate)                    | Near‑vent Plinian, data‑poor                        | Strictly monotonic log‑linear decay              |
| **Power law I**         | α, x_min                    | Fractal fragmentation (phreatomagmatic, Plinian)    | Linear log‑log plot                              |
| **Power law II**        | α, x_min, x_max             | Same as Power law I, but with observable limits     | Log‑log linear + roll‑off at tails               |
| **Weibull / Rosin–Rammler** | k (shape), λ (scale)     | Most eruption types; most versatile         | Unimodal or skewed; k controls shape             |



| Distribution | Equation | Parameters |
|---|---|---|
| Exponential | $$f(\phi) = \lambda \, e^{-\lambda (\phi - \phi_0)}$$ | $\lambda$ = rate parameter (steepness of decay); $\phi_0$ = coarsest grain size (onset phi) |
| Power law I | $$f(\phi) = \frac{\alpha-1}{\phi_{\min}}\left(\frac{\phi}{\phi_{\min}}\right)^{-\alpha}$$ | $\alpha$ = power-law exponent (fractal slope in log-log); $\phi_{\min}$ = lower bound — coarsest clast phi |
| Power law II | $$f(\phi) = \frac{1-\alpha}{\phi_{\max}^{1-\alpha}-\phi_{\min}^{1-\alpha}}\,\phi^{-\alpha}$$ | $\alpha$ = fractal exponent; $\phi_{\min}$, $\phi_{\max}$ = coarse cutoff (largest clast, set by conduit or field observation) and fine cutoff (instrument resolution or aerodynamic settling limit) |
| Weibull / Rosin-Rammler | $$f(\phi) = \frac{k}{\lambda}\left(\frac{\phi}{\lambda}\right)^{k-1}\exp\!\left[-\left(\frac{\phi}{\lambda}\right)^{k}\right]$$ | $k$ = shape parameter (controls sorting and skewness); $\lambda$ = scale parameter (characteristic grain size, related to median) |
