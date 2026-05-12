# ICRL: Learning to Internalize Self-Critique with Reinforcement Learning

This repository will host the official implementation of **ICRL**, a reinforcement learning framework for helping language agents internalize self-critique.

ICRL targets a common limitation of critique-based agent improvement: a model may solve a task after receiving critique, but fail again when the critique is removed. The goal of ICRL is to transfer critique-guided improvements back into the critique-free solver, so the agent improves its underlying capability instead of becoming dependent on external feedback.

<p align="center">
  <img src="assets/method.png" alt="ICRL framework overview" width="90%">
</p>

## Overview

ICRL jointly trains a solver and a critic from a shared backbone:

- The **critic** learns to produce feedback that improves the solver's subsequent attempt.
- The **solver** learns to internalize successful critique-guided revisions into its critique-free behavior.
- A distribution-calibration re-weighting ratio helps avoid blindly imitating behavior that only works under critique-conditioned prompts.

The method is evaluated on agentic and reasoning tasks, including text-world interaction, web navigation, multi-hop question answering, and mathematical reasoning.

## Repository Status

The source code is currently being organized and will be added later.

## Citation

Citation information will be added after the paper metadata is finalized.
