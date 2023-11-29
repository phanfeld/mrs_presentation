---
title: Kidnapping Deep Learning-based Multirotors using Optimized Flying Adversarial Patches
# subtitle: Pandoc revealjs
author: Pia Hanfeld, Khaled Whaba, Marina M.-C. Höhne, Michael Bussmann, Wolfgang Hönig
date: December 3rd, 2023

title-slide-attributes:
    data-background-image: images/title.svg
    data-background-size: contain

minScale: 0.2
maxScale: 10.0
slideNumber: true
navigationMode: 'linear'
controls: false
---
# Motivation
## Real-world adversarial attacks
* Adversarial patches are widely applied in Computer Vision and Autonomous Driving domain


![](images/patch_stop_signs.svg){width=70%}\
[@Eykholt2018]

![](images/patch_cv.svg){width=50%}\
[@Thys2019]

## State of the art
- Current adversarial attacks for UAVs do not negatively affect the control

. . .

- Patches are either static or placed on moving objects close to the ground

## Can we find adversarial patches and an attacker policy that allows for full control over the victim UAV?

# Flying Adversarial Patches
## Scenario

![](images/overview_v7.png)\
Will be replaced!

## The deep learning model under attack

```{=html}
<video data-autoplay src="videos/clip_frontnet.m4v"></video>
```
PULP-Frontnet [@Palossi2022]


## From pattern and position to policy
::: {.r-stack}
:::: {.fragment .current-visible}
<!-- ```{=html}
<img src="images/retrieve_policy_1_1.png" alt="drawing" height="300"/>
``` -->
![](images/retrieve_policy_1_1.png){width=80%}
::::
:::: {.fragment .current-visible}
![](images/retrieve_policy_1_2.png){width=80%}
::::
:::: {.fragment .current-visible}
![](images/retrieve_policy_1_3.png){width=80%}
::::
:::: {.fragment .current-visible}
![](images/retrieve_policy_2_1.png){width=80%}
::::
:::: {.fragment .current-visible}
![](images/retrieve_policy_2_2.png){width=80%}
::::
:::: {.fragment .current-visible}
![](images/retrieve_policy_3.png){width=80%}
::::
:::

## Optimizing the patches and their positions
![](images/schematic_attack_1.svg)

## Target Trajectory
![](images/target_trajectory.svg)

## Assignment
![](images/schematic_attack_2.svg)

## Optimization
![](images/schematic_attack_3.svg){width=65%}

## Optimization
* Compared 3 different optimization algorithms:

![](images/plot_exp1_2.svg){width=49%}
![](images/plot_exp1_3.svg){width=49%}

## Optimization
![](images/plot_exp1_1.svg){width=100%}

## Scalability
![](images/exp2.svg){width=100%}


# Real-world experiments
## Attacker and victim
## 
```{=html}
<video data-autoplay src="videos/only_attacker.m4v"></video>
```
## Person, attacker and victim
## 
```{=html}
<video data-autoplay src="videos/attacker_person.m4v"></video>
```
## An actual kidnapping
## 
```{=html}
<video data-autoplay src="videos/attacker_gate.m4v"></video>
```

# Summary
## Contributions
- Adversarial patches that can be placed anywhere in the environment

- Attacker policy that is able to force victim onto target trajectory

. . .

- Scalable to team of attacker and victims UAVs

. . .

## Thank you for your attention!
Questions? Let's chat during the breaks or feel free to mail me: p.hanfeld@hzdr.de

## References
::: {#refs}
:::
