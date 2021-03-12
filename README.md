# Robust-Adaptive Interval Predictive Control for Linear Uncertain Systems

# Abstract

We consider the problem of stabilization of a linear system, under
state and control constraints, and subject to bounded disturbances
and unknown parameters in the state matrix. First, using a simple
least square solution and available noisy measurements, the set of
admissible values for parameters is evaluated. Second, for the estimated
set of parameter values and the corresponding linear interval model
of the system, two interval predictors are recalled and an unconstrained
stabilizing control is designed that uses the predicted intervals.
Third, to guarantee the robust constraint satisfaction, a model predictive
control algorithm is developed, which is based on solution of an optimization
problem posed for the interval predictor. The conditions for recursive
feasibility and asymptotic performance are established. Efficiency
of the proposed control framework is illustrated by numeric simulations.

----------------------------
# Videos

<p align="center"><iframe width="800" height="400" src="https://www.youtube.com/embed/axurBzHRLGY" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></p>

----------------------------

# Paper and Bibtex

<div style="display: flex;">
<div style="flex: 0 0 15em;">
	<a href="{{ site.paper_url }}">
		<img class="layered-paper-big" src="./assets/images/thumbnail.png">
		<br>
		<h2>[Paper]</h2>
	</a>
</div>
<div style="flex: auto" markdown="1">

## Citation

Leurent, E., Efimov, D., and Maillard, O-A., 2020.<br>
*Robust-Adaptive Interval Predictive Control for Linear Uncertain Systems.* In 59th Conference on Decision and Control.

## [[Bibtex]]()

```
@inproceedings{Leurent2020robust,
	author = {Leurent, Edouard and Efimov, Denis and Maillard, Odalric-Ambrym},
	title = {{Robust-Adaptive Interval Predictive Control for Linear Uncertain Systems}},
	booktitle = {2020 IEEE 59th Conference on Decision and Control (CDC)},
	address = {Jeju Island, Republic of Korea},
	month = Dec,
	year = {2020},
}
```
</div>
</div>

----------------------------
# Instructions

## Installation

```shell
pip install -r requirements.txt
```

1. Install the [rl-agents](https://github.com/eleurent/rl-agents) implementations, and clone the repository.
2. Install the [highway-env](https://github.com/eleurent/highway-env) environment

## Instructions

The experiments can be reproduced by running:

```shell
cd <path-to-rl-agents>/scripts
python experiments.py configs/LaneKeepingEnv/env.json configs/LaneKeepingEnv/agents/constrained_epc.json --train
```

The results will appear in the `scripts/out` directory.

----------------------------

# Acknowledgements

This work was supported by the French Ministry of Higher Education and Research, and CPER Nord-Pas de Calais/FEDER DATA Advanced data science and technologies 2015-2020.
