# Experiment 7 – how the results were produced

Simulator: **Python 2-D kinematic re-implementation (NumPy) of the webots-robotics-sim worlds** — Webots was
not installed. Python 3.10.0, NumPy 1.26.4, Matplotlib 3.10.5 · OS: Windows 11 (10.0.26300) · CPU: Intel64 Family 6 Model 170.

```bash
python -m jupyter nbconvert --to notebook --execute --inplace exp07.ipynb    # or Kernel > Restart & Run All
```

`exp07.ipynb` contains the simulator (same arena/obstacle geometry, start poses, 32 ms step, Braitenberg
weights, follow-the-gap steps, wheel parameters, IR lookup table and 180-beam lidar as the repository), runs
16 settings x 3 repeats (SEED = 9327), writes `runs/<world>__<setting>__r<k>.csv`, and makes all tables
(`tables/`) and figures (`figs/`). Runtime about 2 min.

Differences from Webots: no 3-D rigid-body physics (round bodies pushed out of obstacles, friction factor 0.3
on contact); repeats differ by seeded start-pose jitter and sensor noise. Figure 7.1 is a rendered top-down
snapshot of the simulation, not a Webots window screenshot.

Exercises attempted (GUIDE.md §10): **1 – Speed vs safety** (cruise sweep 0.2–1.0) and
**2 – Swap the wiring** (aggressive vehicle, `wiring=-1`).
