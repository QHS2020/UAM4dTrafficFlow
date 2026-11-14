# UAM4dTrafficFlow

A **multiclass 4-D continuum model and solver** for Urban Air Mobility (UAM) traffic
flow with **obstacle awareness**.

The model describes the macroscopic flow of eVTOL aircraft as a multiclass density
field over a 4-D space-time grid (three spatial dimensions + time). Routing is solved
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

---

## Study area & obstacles

<p align="center">
  <img src="figs/air_corridor.jpg" width="700" alt="Air corridor concept">
  <br><em>The air-corridor concept over the study area.</em>
</p>

<p align="center">
  <img src="figs/Buildings_sg.jpg" width="700" alt="Singapore buildings">
  <br><em>Singapore building footprints — the obstacles the solver routes around.</em>
</p>

## Fundamental diagram

<p align="center">
  <img src="figs/Drew_FD.jpg" width="520" alt="Drew fundamental diagram">
  <br><em>The Drew fundamental diagram (density → speed).</em>
</p>

<p align="center">
  <img src="figs/Drew_FD_NoCongestionBranch.jpg" width="520" alt="Drew FD no-congestion branch">
  <br><em>The no-congestion branch of the Drew FD.</em>
</p>

<p align="center">
  <img src="figs/fd_continuum.jpg" width="520" alt="Continuum fundamental diagram">
  <br><em>The fundamental diagram used by the continuum solver.</em>
</p>

## Solver results

<p align="center">
  <img src="figs/plot_density_timeseries.png" width="700" alt="Density timeseries">
  <br><em>The solved density field <code>rho_total</code> over time.</em>
</p>

<p align="center">
  <img src="figs/potential.jpg" width="700" alt="Eikonal routing potential">
  <br><em>The Eikonal routing potential field.</em>
</p>

---

## License

[GPL-3.0-or-later](LICENSE) — the license file accompanies the source-code release.
