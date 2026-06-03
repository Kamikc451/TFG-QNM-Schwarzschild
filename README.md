TFG-QNM-Schwarzschild

Python codes developed for the Bachelor's Thesis:

Numerical study of quasi-normal modes of Schwarzschild black holes

Author: Óscar Notario Poveda
Bachelor's Degree in Physics
Universidad de Alicante
Academic year: 2025-2026

Description

This repository contains the Python scripts used to obtain the numerical results presented in the thesis. The work focuses on the computation of quasi-normal modes of Schwarzschild black holes using two numerical methods:

direct integration of the Regge-Wheeler equation by shooting and matching;
Leaver's continued fraction method.

The codes were developed as part of the numerical implementation described in the thesis.

Repository structure
integracion_directa/
    integracion_directa.py

metodo_leaver/
    leaver_60_modos.py
    construccion_semillas_leaver.py

requirements.txt
README.md
LICENSE
Contents
integracion_directa/

Contains the implementation of the direct integration method. The code constructs asymptotic solutions near the horizon and at infinity, integrates them towards a matching point and finds the quasi-normal frequencies by imposing the vanishing of the Wronskian.

It also includes the reconstruction of the radial solution associated with the calculated frequency.

metodo_leaver/

Contains the implementation of Leaver's continued fraction method.

leaver_60_modos.py: final script used to compute the first 60 modes for the families (\ell=2) and (\ell=3), using the refined initial seeds.
construccion_semillas_leaver.py: auxiliary script showing the interpolation and continuation procedure used during the construction of the initial seeds for the higher overtones.
Dependencies

The codes require:

numpy
scipy
matplotlib

They can be installed with:

pip install -r requirements.txt
Notes

The comments inside the code are written in Spanish, following the language of the thesis. The implementation is intended to accompany the explanations given in the written report, where the numerical methods are described step by step.

License

This repository is distributed under the MIT License.
