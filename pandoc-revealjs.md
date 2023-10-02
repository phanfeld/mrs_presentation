---
title: Slide Examples
subtitle: Pandoc revealjs
author: Wolfgang Hönig
date: October, 2023
---

# Layout

## Lists

- Item1
- Item2
- Item3 with *important* text

## Enumerations

1. Item1
2. Item2
3. Item3 with *important* text

## Columns

::: {.container}
:::: {.col}
Column 1  
abc
::::
:::: {.col}
Column 2  
abc
::::
:::


::: {.container}
:::: {.col}
Column a  
abc
::::
:::: {.col}
Column b
::::
:::: {.col}
Column c  
abc
::::
:::

## Blocks

::: {.box-def}
:::: {.box-def-title}
Normal block with title
::::
text
:::

::: {.box-def}
Normal block without title
:::

# Multimedia

## Picture

![](images/robotics.svg)

## Math

$$
\begin{align}
\arg\min_{T, u(t), q(t)} \quad J(T, u(t), q(t)) \quad \text{s.t.}\\
q(0) = q_{start} \quad q(T) = q_{goal}\\
\mathcal{B}(q(t)) \subset \mathcal{W}_{free} \quad \forall t \in [0, T]\\
\dot q(t) = f(q(t), u(t)) \quad \forall t \in [0, T)
\end{align}
$$

## Video

```{=html}
<video data-autoplay src="videos/cubic-bezier.mp4"></video>
```

<!-- Full screen video -->
## 

```{=html}
<video data-autoplay src="videos/cubic-bezier.mp4" width="100%"></video>
```

## Source Code

```python
def Astar(G, d, v_s, v_z, h):
    O = queue()
    while O not empty:
        # smallest f-value
        v = O.pop()
        if v = v_z:
            return solution
        for n in v.neighbor:
        # ...
```

# Animations

# Misc

## References

Great robotics books [@springerHandbook; @lavallePlanningBook]

# References

::: {#refs}
:::

# Appendix

Some appendix at the end