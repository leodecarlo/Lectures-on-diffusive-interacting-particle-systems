# Lectures on Diffusive Interacting Particle Systems

Lecture notes and slides from minicourses delivered at the **Instituto Superior Técnico (IST), University of Lisbon**, and the **Scuola Normale Superiore (SNS), Pisa**.

The material introduces the hydrodynamic scaling of diffusive interacting particle systems (IPS), beginning with the symmetric simple exclusion process and continuing toward geometric decompositions of microscopic currents, non-gradient models, and exclusion processes with vorticity.

The notes are aimed at graduate students and researchers in probability, stochastic processes, mathematical physics, and partial differential equations.

## Repository contents

### 1. [Introduction](intro.pdf)

Three handwritten introductory pages that set up the general framework:

- interacting particle systems on discrete lattices and tori;
- particle configurations and occupation variables;
- conserved quantities and empirical density fields;
- the passage from microscopic stochastic dynamics to macroscopic evolution equations;
- the programme of the minicourses: Chapter 4 of Kipnis and Landim, a review of known results through discrete exterior calculus, and the author's results on microscopic currents and vorticity.

These pages provide a short orientation before the more technical lectures.

### 2. [Hydrodynamics of the SSEP - Chapter 4 of Kipnis-Landim](ch4KL.pdf)

Eighteen handwritten pages devoted to the hydrodynamic limit of the **symmetric simple exclusion process (SSEP)**, following Chapter 4 of Kipnis and Landim and using Billingsley's *Convergence of Probability Measures* for the background on weak convergence, tightness, and probability measures on trajectory spaces.

Topics include:

- the SSEP on the discrete torus and its infinitesimal generator;
- Bernoulli product measures, reversibility, and conservation of the number of particles;
- empirical measures and their interpretation as macroscopic density profiles;
- diffusive time scaling and the emergence of the heat equation;
- probability measures on trajectory spaces and the Skorokhod topology;
- compactness, tightness, Prokhorov-type criteria, and martingale estimates;
- Dynkin's formula and the martingale decomposition of empirical observables;
- characterization of subsequential limit points;
- identification of the limiting density as a weak solution of the heat equation;
- uniqueness of the macroscopic equation and completion of the hydrodynamic-limit argument.

This document gives the probabilistic proof strategy underlying the law of large numbers for the empirical density.

### 3. [Diffusive IPS and discrete Hodge decompositions](IPSdiffusivi/ips_diffusivi%2Bdec.pdf)

A seventeen-slide lecture connecting hydrodynamic limits with geometric decompositions of microscopic currents.

The slides cover:

- motivations for using stochastic lattice gases as models of nonequilibrium systems;
- exclusion dynamics on a periodic lattice and translation-covariant rates;
- invariant measures and reversible dynamics;
- empirical measures, conservation laws, and Fick's law;
- instantaneous and time-integrated microscopic currents;
- the gradient condition and the standard heuristic derivation of hydrodynamics;
- the local-equilibrium replacement principle;
- discrete differential forms on the two-dimensional torus;
- gradient, circulation, and harmonic components in the discrete Hodge decomposition;
- the non-gradient problem and the role of functional Hodge decompositions for translation-covariant local currents;
- the appearance of divergence-free microscopic currents and their possible macroscopic effects.

### 4. [Exclusion processes with vorticity](IPSdiffusivi/model%20with%20vorticity.pdf)

A twenty-seven-page slide deck presenting a non-reversible diffusive exclusion process with an explicit vortical component.

The document develops:

- the generator and transition rates of a two-dimensional exclusion process with local rotations;
- the interpretation of clockwise and anticlockwise particle motion around lattice faces;
- invariance of Bernoulli product measures despite non-reversibility;
- the empirical density and its hydrodynamic limit;
- the integrated empirical current as a distribution-valued trajectory;
- Sobolev spaces and the topology used for current convergence;
- tightness and characterization of limit points for the current field;
- the decomposition of the macroscopic current into dissipative and divergence-free parts;
- a generalized Fick law with an antisymmetric contribution to the diffusion matrix;
- why vorticity affects the limiting current while leaving the density equation unchanged;
- open problems involving numerical tests, current fluctuations, entropy production, and non-gradient models.

Some pages include handwritten diagrams and annotations illustrating the microscopic circulation mechanism.

## Suggested reading order

1. Start with `intro.pdf` for the microscopic-to-macroscopic viewpoint.
2. Read `ch4KL.pdf` for the standard hydrodynamic limit of the SSEP.
3. Continue with `ips_diffusivi+dec.pdf` for microscopic currents and Hodge decompositions.
4. Finish with `model with vorticity.pdf` for the non-reversible model and its current hydrodynamics.

## Main mathematical themes

### Hydrodynamic scaling

The microscopic dynamics evolves on a lattice of mesh size of order `1/N`, while time is accelerated by `N^2`. Under suitable assumptions, the random empirical density converges to a deterministic profile solving a diffusion equation.

### Density and current

The empirical density satisfies a microscopic continuity equation. Its associated current contains more information than the density alone: divergence-free parts disappear from the density equation but remain visible in the limiting current field.

### Gradient and non-gradient systems

For gradient systems, the instantaneous current can be written as a discrete gradient of a local function, making the hydrodynamic equation comparatively direct to identify. In non-gradient systems, the current requires additional approximation or variational arguments. The functional Hodge viewpoint separates gradient, circulation, and harmonic contributions.

### Vorticity

The model with vorticity provides an explicit non-reversible example whose invariant measure is still a Bernoulli product measure. Its macroscopic current contains an antisymmetric, divergence-free term. Consequently, the density follows the usual diffusion equation even though the current retains a rotational component.

## References

### Probability and weak convergence

- P. Billingsley, *Probability and Measure*, 3rd ed., Wiley, 1995. A foundational reference for measure-theoretic probability, laws of large numbers, conditional expectations, and martingales. See also the [Wiley Anniversary Edition](https://www.wiley.com/en-us/Probability+and+Measure%2C+Anniversary+Edition-p-9781118341919).
- P. Billingsley, *Convergence of Probability Measures*, 2nd ed., Wiley, 1999. The principal background reference for weak convergence, tightness, and probability measures on function spaces. [DOI: 10.1002/9780470316962](https://doi.org/10.1002/9780470316962).

### Hydrodynamic limits

- C. Kipnis and C. Landim, *Scaling Limits of Interacting Particle Systems*, Grundlehren der mathematischen Wissenschaften 320, Springer, 1999. In particular, Chapter 4 develops the hydrodynamic equation for the symmetric simple exclusion process. [DOI: 10.1007/978-3-662-03752-2](https://doi.org/10.1007/978-3-662-03752-2).
- H. Spohn, *Large Scale Dynamics of Interacting Particles*, Springer, 1991. [DOI: 10.1007/978-3-642-84371-6](https://doi.org/10.1007/978-3-642-84371-6).

### Related work by Leonardo De Carlo

- L. De Carlo, **Geometrical Structures of the Instantaneous Current and Their Macroscopic Effects: Vortices and Perspectives in Non-gradient Models**, in C. Bernardin, F. Golse, P. Gonçalves, V. Ricci, and A. J. Soares (eds.), *From Particle Systems to Partial Differential Equations*, Springer Proceedings in Mathematics & Statistics 352, pp. 169-193, 2021. [Springer chapter](https://doi.org/10.1007/978-3-030-69784-6_9) | [arXiv:2004.01548](https://arxiv.org/abs/2004.01548).
- L. De Carlo, D. Gabrielli, and P. Gonçalves, **Hydrodynamic Limit of an Exclusion Process with Vorticity**, *Annales de l'Institut Henri Poincaré, Probabilités et Statistiques* 61(1), 232-257, 2025. [DOI: 10.1214/23-AIHP1441](https://doi.org/10.1214/23-AIHP1441) | [arXiv:2109.07897](https://arxiv.org/abs/2109.07897).
- L. De Carlo and D. Gabrielli, **Gibbsian Stationary Non-equilibrium States**, *Journal of Statistical Physics* 168, 1191-1222, 2017. [DOI: 10.1007/s10955-017-1852-5](https://doi.org/10.1007/s10955-017-1852-5) | [arXiv:1703.02418](https://arxiv.org/abs/1703.02418).

## Author

**Leonardo De Carlo**

## Note on the material

The repository preserves the lecture material in its original form. The handwritten notes are scans, while the remaining documents are presentation slides, in some cases supplemented by handwritten annotations.
