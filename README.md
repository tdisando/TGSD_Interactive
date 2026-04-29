# TGSD_Interactive
Exploring three distribution curves for characterising pyroclastic deposits

## About the models
Inspired by study of radioactive decay from Rutherford and Soddy (1902; https://doi.org/10.1080/14786440209462856) and sequence of random events from Poisson (1837; https://doi.org/10.48550/arXiv.1902.02782), fractal fragmentation theory (pure and truncated Paretos) from Turcotte (1986; https://doi.org/10.1029/JB091iB02p01921) and Kaminski and Jaupart (1992; https://doi.org/10.1029/98JB02795), and  material failure test from Weibull (1939; https://doi.org/10.1115/1.4010337) and crushing coal from Rosin and Rammler (1933; https://doi.org/10.1007/BF01439773).

| Distribution            | Parameters                 | Ideal eruption style                               | Key diagnostic                                   |
|-------------------------|-----------------------------|-----------------------------------------------------|--------------------------------------------------|
| **Exponential**         | λ (rate)                    | Near‑vent Plinian, data‑poor                        | Strictly monotonic log‑linear decay              |
| **Power law I**         | α, x_min                    | Fractal fragmentation (phreatomagmatic, Plinian)    | Linear log‑log plot                              |
| **Power law II**        | α, x_min, x_max             | Same as Power law I, but with observable limits     | Log‑log linear + roll‑off at tails               |
| **Weibull / Rosin–Rammler** | k (shape), λ (scale)     | Most eruption types; default recommendation          | Unimodal or skewed; k controls shape             |

Trying to understand:
- Deposit-based distributions of tephras in natural cases
- An approach to magma fragmentation, yet ideally without atmospheric disturbances
