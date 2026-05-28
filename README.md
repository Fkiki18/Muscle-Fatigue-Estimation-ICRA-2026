# Muscle Fatigue Estimation in Physical Human–Robot Interaction

> A data-driven framework for continuous muscle fatigue estimation during cyclic pHRI tasks using surface EMG signals and machine learning regression models.

---

## Overview

This work presents a machine learning framework for estimating muscle fatigue
in physical human–robot interaction (pHRI) tasks using surface EMG (sEMG) signals.
Several regression models — including Random Forest, XGBoost, Linear Regression,
and a CNN — were trained to continuously track fatigue progression rather than
classify discrete fatigue states. Experiments were conducted with human participants
interacting with a collaborative robot performing cyclic arm movements. The models
were also tested on unseen movement directions to evaluate cross-task generalization.

<p align="center">
  <img src="System Workflow.png" width="700" alt="Experimental setup showing a human participant interacting with a collaborative robot while wearing sEMG sensors on the arm"/>
  <br>
  <em>Experimental setup: human participant interacting with a collaborative robot under admittance control, with sEMG sensors attached to the arm.</em>
</p>

---

## Methods

- **Sensors:** Surface EMG (sEMG) placed on the human arm
- **Target variable:** Fraction of Cycles to Fatigue (FCF) — a continuous regression target
- **Features:** Three frequency-domain + one time-domain EMG features; spectrogram representations for CNN
- **Models compared:**
  - Random Forest
  - XGBoost
  - Linear Regression
  - Convolutional Neural Network (CNN)
- **Robot:** Collaborative robot driven by an admittance controller
- **Task:** Lateral (left-right) cyclic movements until muscular exhaustion; cross-task tests on vertical and circular movements

---

## Key Contributions

- Frames fatigue estimation as a **regression problem** rather than classification, enabling tracking of gradual physiological changes
- Demonstrates **cross-task generalization**: models trained on lateral movements generalize to vertical and circular unseen tasks
- Provides subject-specific ML models suitable for **adaptive control and timely intervention** in pHRI

---
<p align="center">
  <img src="ICRA 2026 Poster.jpg" width="700" alt="Experimental setup showing a human participant interacting with a collaborative robot while wearing sEMG sensors on the arm"/>
  <br>
  <em>Experimental setup: human participant interacting with a collaborative robot under admittance control, with sEMG sensors attached to the arm.</em>
</p>


<p align="center">
  <img src="ICRA Graphical Abstract.jpg" width="700" alt="Experimental setup showing a human participant interacting with a collaborative robot while wearing sEMG sensors on the arm"/>
  <br>
  <em>Experimental setup: human participant interacting with a collaborative robot under admittance control, with sEMG sensors attached to the arm.</em>
</p>
