# Fetal Circulation Mechanistic Model

Mechanistic 0D model of fetal circulation and cardiovascular development across gestation.

## Overview

This project builds upon the 0D fetal circulation model developed by **Mª Inmaculada Villanueva-Baxarias et al. (2025)**, which provides a reference parameterization for a healthy fetus at **36 weeks of gestation**.

The present framework extends the original model by introducing physiologically motivated gestational-age-dependent scaling laws, allowing the simulation of cardiovascular development throughout gestation. In addition, several variability modules are implemented to study different sources of physiological variability.

The framework is intended to investigate normal fetal cardiovascular physiology, developmental hemodynamics, and the generation of virtual fetal populations.

## Features

- Gestational-age-dependent parameter scaling
- Fetal weight and percentile-based adaptation
- Placental growth and maturation scaling
- Hemodynamic simulations of the fetal circulation
- Cardiac pressure, volume, and flow analysis
- Doppler-derived indices (MPI, E/A, PI, ETF, FTF)
- Vessel velocity and wall shear stress computation
- Validation against fetal echocardiography and Doppler literature
- Physiological variability analysis

## Repository structure

### `MODEL_GA_FETAL`
Baseline gestational-age scaling model.

- Simulates cardiovascular development across gestation.
- Implements the standard scaling framework.
- Used to obtain the reference hemodynamic results.

### `MODEL_VAR_JUP`
Fetal growth variability model.

- Includes the standard gestational-age scaling.
- Introduces fetal weight and percentile variability.
- Generates different physiologically plausible fetal states.

### `MODEL_VAR_JUP_PLACENTA`
Placental variability model.

- Includes gestational-age scaling.
- Introduces variability vascular resistance and compliance.
- Studies the influence of placental development on fetal hemodynamics.

### `MODEL_VAR_JUP_BRAIN`
Cerebral maturation variability model.

- Includes gestational-age scaling.
- Introduces variability in cerebral circulation parameters.
- Evaluates the effects of brain maturation on the overall cardiovascular system.

## Reference

Villanueva-Baxarias, M. I., et al. (2025).

*0D fetal circulation model parameterized for a healthy fetus at 36 weeks of gestation.*

## Purpose

This framework provides a first-order approximation of normal fetal cardiovascular development and constitutes a first step toward the generation of virtual fetal populations and patient-specific computational models.
