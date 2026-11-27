# aisr-lab-<SAP ID> — CSAI4014 Algorithms for Intelligent Systems and Robotics, Laboratory

| | |
|---|---|
| Name | `<Suhani Baderia>` |
| SAP ID / Roll no. | `<500119327>` / `<R2142230288>` |
| Batch | `<4>` (B.Tech CSE AI & ML, Semester VII, Autumn 2026–27) |
| Course teacher | Dr. Resham Raj Shivwanshi |

## Layout

```
exp01-signals/    exp01.ipynb  figs/  tables/   Time & frequency domain, pendulum
exp02-queens/     exp02.ipynb  figs/  tables/   Eight queens (brute force vs backtracking)
exp03-search/     exp03.ipynb  figs/  tables/   BFS and DFS on a grid maze
exp04-hillclimb/  exp04.ipynb  figs/  tables/   Hill climbing, random restarts
exp05-rl/         exp05.ipynb  figs/  tables/   Tabular Q-learning
exp06-neural/     exp06.ipynb  figs/  tables/   2-layer neural network (NumPy) on XOR
exp07-webots/     exp07.ipynb  controllers/ (changed files)  runs/*.csv  worlds/  figs/  NOTES.md
exp08-xembody/    results/*.csv  figs/  exercises/  NOTES.md
```

Every notebook runs top to bottom on a fresh kernel (`Kernel > Restart & Run All`) and writes its
figures to `figs/` and observation tables to `tables/`.

## Requirements

Python 3.10+, NumPy, SciPy, Matplotlib (Exp. 1–7); Webots R2025a (Exp. 7); PyBullet in the
`aisr-xembody` environment (Exp. 8).

```bash
pip install numpy scipy matplotlib jupyter
```

## Sources and AI tools used

| Source / tool | Used for |
|---|---|
| AISR Laboratory Manual, Chapters 2–7 | Experiments 1–6 (aims, procedure, questions) |
| github.com/reshamrajs/webots-robotics-sim (README.md, GUIDE.md) | Experiment 7 |
| AISR-Cross-Embodiment-PyBullet (README.md, MANUAL.md) | Experiment 8 |
| NumPy / SciPy / Matplotlib documentation | All |
| `<add any other source>` | |
