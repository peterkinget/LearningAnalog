# SOLUTION: Pre-Requisites Test for Analog Electronic Circuits

## Circuit Analysis
1. Analysis of RC Networks

* Bode Plots of transfer function $H(j 2\pi f)$
    - Small Signal AC analysis `.ac`

![schematic_H_ac](img/schematic_H_ac.png)
![results_H_ac](img/results_H_ac.png)

* Response to a Sine Wave
    - Transient simulation `.tran` with a sinusoidal input signal

![schematic_H_ac](img/schematic_H_sine.png)
![results_H_ac](img/results_H_sine_transient.png)
![results_H_ac](img/results_H_sine_steady_state.png)

* Extra: Impulse Response 
    - Transient simulation `.tran` with a step input created with a PWL source
    
![schematic_H_ac](img/schematic_H_impulse.png)
![results_H_ac](img/results_H_impulse.png)

3. Analysis of Impedance

* Bode Plots of transfer function $Z(j 2\pi f)$
    - Small Signal AC analysis `.ac`
    
![schematic_H_ac](img/schematic_Z.png)
![results_H_ac](img/results_Z.png)