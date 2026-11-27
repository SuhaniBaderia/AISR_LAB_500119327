# Experiment 8 – how the results were produced

Simulator: **NumPy kinematic simulation** (PyBullet not used). Python 3.10.0, NumPy 1.26.4, Matplotlib 3.10.5 ·
OS: Windows 11 (10.0.26300) · CPU: Intel64 Family 6 Model 170.

```bash
python -m jupyter nbconvert --to notebook --execute --inplace exp08.ipynb    # about 4 min
```

Arms (DH models): KUKA LBR iiwa 7, Franka Panda (Craig DH), UR5, and a compact 5-DOF arm (generic, approximate).
Skill: pick a 5 cm cube and place it on a goal; scripted expert through damped-least-squares IK.
Policies: NumPy MLP (2 x 128 tanh, Adam) trained by behaviour cloning; SEED = 9327, 150 demos per arm, 50 test tasks.

Outputs: `results/T8_1…T8_5*.csv`, `results/01_workspace.png … 05_multi_embodiment.png` (copied to `figs/`).

Exercises (`exercises/`): **A – observation-noise robustness**, **B – data efficiency (number of demos)**.
These were chosen without MANUAL.md; rename them to the matching E1–E6 numbers (or replace) once the manual is available.
