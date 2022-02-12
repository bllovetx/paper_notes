---
layout: post
date: 2022-02-12
author: 曾许曌秋
title: atom-atom entanglement
tags: 
    - BSM
    - cavity
    - STIRAP
    - Rb87
header-img: /note_pics/22-02-12-atom-atom-entanglement.png

---

# atom-atom entanglement

> 2022-02-12
> 
> 曾许曌秋

## paper list

[a] [quantum networking of neutral atom processor](/Important_papers/an_architecture_for_quantum_networking_of_neutral_atom_processor.M_Saffman.2022.arxiv/2202.01634.pdf)

[b] [photon atom entanglement](/Important_papers/observation_of_entanglement_of_a_single_photon_with_a_trapped_atom.Harald_Weinfurter.2006.prl/PhysRevLett.96.030404.pdf)

## abstract

### 1. photon atom entanglement: preparation and verification

![rb87 entanglement level](/note_pics/22-02-12-rb87-entanglement-level.png)

Rb87 is first initialized at F=1, $m_F$=0, and then excited to $^2P_{3/2}$, F'=0 state with a 30ns $\pi$ pulse. By collecting emitted photon along the quantization axis, $\lvert\psi\rangle=\frac{1}{\sqrt{2}}(\lvert m_F=-1\rangle\lvert\sigma^+\rangle+\lvert m_F=+1\rangle\lvert\sigma^-\rangle)$ is obtained.

Entanglement is verified with a state selective stimulated Raman adiabatic passage (STIRAP) in [b], where STIRAP is illustrated below.

![STIRAP](/note_pics/22-02-10-stirap.jpg)

Here by state selective STIRAP, a superposition of $m_F=\pm1$ is selected as $g_1$ state and thus orthogonal component will not be affected. Projective component is adiabatically transformed to F=2 and removed by transition from F=2 to F'=3

![selective STIRAP](/note_pics/22-02-12-illustration-of-selective-STIRAP.png)

Visibility of 0.74 $\pm$ 0.01 is achieved violating CHSH inequality and by reconstruction, pure state entanglement is illustrated below.

![pure state entanglement](/note_pics/22-02-12-pure-state-entanglement.png)

Repetition rate is $1.25\times10^5s^{-1}$

### 2. improvement and BSM

Paper [a] theoretically analyses improvements to photon collecting process and states achievable rate and fidelity to be 5800$s^{-1}$ and 0.91 respectively compare to former results below.

![former rate and fidelity of remote entanglement of matter qubits](/note_pics/22-02-12-former-results.png)

To optimize the photon collection efficiency, cavity with proper parameters is used. This including optimizing cavity length(4-10mm), mirrors radius of curvature, transition rate of two mirror, atom position in cavity.

### 3. possible problem

Paper [a] seems too ideal and many problem may be severe in real experiments. 

Despite of some detailed problem, two photon will not emitted at the same time. From the process of experiment decribed in paper, window of entire 1$\mu$s may be used. This seem a long time but the paper claimed influence to fidelity caused by temporal overlap of photons to be less 0.2%. Former work on this protocal may be referred to check this.

## interesting things

### 1. about H.Weinfuter

The experiment [b] is authored by Harald Weinfurter, who is also the author of [frustrated interferometer](/Important_papers/frustrated_interference.Herzog.1993.PRL/PhysRevLett.72.629.pdf)(see former notes).

He graduated from Technical University of Vienna and worked at Ludwig Maximilians University in Munich before and now working at mpq.

There are many influential paper that is authored by him together with Pan/Lu. Many important work of quantum optics, quantum information are conducted by him.

### 2. experimental detail of [b]

> For the dipole trap waist size of 3.5$\mu$m, a collisional blockade mechanism ensures that only single atoms are captured

overall detection efficiency: $5\times10^{-4}$

### 3. collective efficiency with different N.A. alone quantization axis

![efficiency alone quantization axis](/note_pics/22-02-12-efficiency-along-quantization-axis.png)

Overlap between sigma light and gaussian light seem satisfactory.

> note: our current experiment collect photon perpendicular to quantization axis, both overlap and collective efficiency of lens decrease severely. Though we have discussed this before, importance of rediscussion still exists to imporve our collective efficiency.



## Suggestion on further experiments

Realize **frequency multiplexing** by addressing different atom with different intensity to match cavity mode?

cavity length permits or not?

> after rough calculation, 10mm correspond to 30GHz FSR. This should be possible but relatively large with addressing of  (near-)resonant light. Specifically, in [experiment of Thompson with Er in solid-state](/Important_papers/parallel_single-shot_measurement_and_coherent_control_of_solid-state_spins_below_the_diffraction_limit.SongtaoChen=Thompson.2020.science/science.abc7821.pdf), around 10GHz is shifted with AC stark shift.

![ac stark shift of Er](/note_pics/22-01-20-ion-spectrum.png)

Butterfly cavity may be used to reduce FSR?