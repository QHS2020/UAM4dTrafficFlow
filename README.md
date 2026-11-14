# UAM4dTrafficFlow

A **multiclass 4-D continuum model and solver** for Urban Air Mobility (UAM) traffic
flow with **obstacle awareness**.

The model describes the macroscopic flow of eVTOL aircraft as a multiclass density
field over a 4-D space-time grid (three spatial dimensions + time).  Routing is solved
with a fast Eikonal-based method, and the space-time grid is **obstacle-aware** —
buildings and terrain are treated as impenetrable cells (via a validity mask), so
traffic naturally routes around them.

## Paper

> **Multiclass 4D Continuum model and solver for Urban Air Mobility Traffic Flow with
> obstacle awareness**
>
> *Submitted to the 2027 IEEE Intelligent Vehicles Symposium (IV).*

The full source code will be released here **after the paper is accepted**. Until then,
this repository contains the paper's figures and this overview only.

## Figures

| file | description |
|---|---|
| `air_corridor.jpg` | the air-corridor concept over the study area |
| `Buildings_sg.jpg` | Singapore building footprints (the obstacles) |
| `Drew_FD.jpg` | the Drew fundamental diagram (density → speed) |
| `Drew_FD_NoCongestionBranch.jpg` | the no-congestion branch of the Drew FD |
| `fd_continuum.jpg` | the fundamental diagram used by the continuum solver |
| `plot_density_timeseries.png` | the solved density field `rho_total` over time |
| `potential.jpg` | the Eikonal routing potential field |

## License

[GPL-3.0-or-later](LICENSE) — the license file accompanies the source-code release.
