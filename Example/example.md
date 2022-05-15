---
title: Keynote
separator: ---
verticalSeparator: -v-
theme: white
revealOptions:
    transition: fade
---

<!-- .slide: data-transition="zoom" -->
## Empirical Models of Demand

<div style="margin-bottom:1cm;"></div>

<div style="font-size:30pt; padding-bottom:1.5cm">Industrial Organization 101</div>

[Hao-Che Hsu](https://www.haochehsu.com/)

Note: speaker note for page 1

---

<h3>This is...</h3>

<div class="r-stack">
  <div>A brief </div> <!-- .element: class="fragment fade-in-then-out" -->
  <div>overview</div> <!-- .element: class="fragment fade-in-then-out" -->
  <span class="fragment fade-in">
    <span class="fragment highlight-red">
      <span class="fragment fade-out">
        presented by web slides
      </span>
    </span>
  </span>
  <span class="fragment fade-in-then-out" style="width: 80%;">
    with <b>Javascript<b><br>
    <img src="js_logo.png" />
  </span>
</div>

Note: speaker note for page 1

---

<!-- .slide: data-transition="concave" -->
Nevigate with the <span style="color:green;">4-directional controler</span> on the bottom right corner

or use the keyboard <span style="color:green;">4 arrow keys</span>.

---

<!-- .slide: data-transition="zoom" -->

# IO, What is it about? 

-v-

<div style="text-align: left; padding-left:5cm">

Focuses on industries in our Economy:<br><br>

<div style="line-height:80px">

* Structure <!-- .element: class="fragment data-fragment-index="1" -->
* Firms behavior <!-- .element: class="fragment data-fragment-index="2" -->
* Individuals <!-- .element: class="fragment data-fragment-index="3" -->

</div>
</div>

---

<!-- .slide: data-transition="convex" -->

## Method: Structural Modeling

<div style="line-height:120px">

1. Build a theoretical model of market participants
2. Use industry data to estimate the parameters
3. Use estimates to conduct conterfactual evaluations

</div>

---

## 3 steps of Structure Modeling Process <br><br>

[Step 1](#/5/1) &nbsp; | &nbsp; [Step 2](#/5/2) &nbsp; | &nbsp; [Step 3](#/5/3)

-v-

### Step1: Industry descriptive analysis

- Learn about the industry e.g. from news, industry sources

- Collect data trying to understand key facts, aspects of the industry and firm behavior

<div style="margin-bottom:1cm;"></div>

<small>[Go back](#/5)<small>

-v-

### Step2: Acquiring industry data

<div style="text-align: left;">
In our data... 

- $y$ : observable data on economic outcomes determined by firm or consumer behavior. e.g. quantity($Q$), price($P$)

- $x$ : observable data on enviornment exogenous features. e.g. number of consumers in the market, their incomes

- Data can be characterized as a conditional distribution $G(y|x)$
</div>

<div style="margin-bottom:1cm;"></div>

<small>[Go back](#/5)<small>

-v-

### Step3: Model construction

<div style="font-size:25pt; text-align: left; line-height:70px">

- Based on Economic **theory**, we write an **model**:
    - $\text{agents}\xrightarrow{\tiny \text{payyoff} \Longrightarrow \text{make choices} }$ outcome/behavior $y$
    - consumers choose what to buy $\rightarrow$ determine quantity sold
- Behavior(choice): results from optimizing given payoffs
- Payoffs for agents is a function of:
    - choices of all market participants
    - exogenous observables: $x$, unobserved factors: $u \sim F$
- Model results in a structural relationship (<span style="color:blue">Koopmans and Reiersol, 1950</span>): $\phi(y,x,u)=0$

</div>

<div style="margin-bottom:1cm;"></div>

<small>[Go back](#/5)<small>

---

### Structural Model v.s Reduced Form

-v-

<div style="font-size:25pt;line-height:50px">

### Suppose <span style="color:purple">Verizon</span> and <span style="color:purple">AT&T</span> want to merge:

- **Reduced form** researcher:
    - Look at quasi-random mergers. e.g. exploiting court rulings, search for merger news, and estimate the treatment effect of mergers from historical data.

- **Structural** researcher:
    - Build a model of national mobile telecom market, estimate features of demand and costs. Then evaluate the counterfactual where Verizon and AT&T merge.
</div>

---

### Nested Logit Model

<div style="font-size:25pt;line-height:70px">

- Goldberg (1995) and Goldberg (1998)
- $u_{ij}=x_j\beta+z_g\gamma-\alpha_ip_j+\epsilon_{ij}$ where $\epsilon_{ij}=\zeta_{ig}+(1-\sigma_g)\nu_{ij}$
    - utility of choice $j$ in nest $g$ for individual $i$
    - $\zeta_{ig}$ is common to all alternatives in nest $g$, it's distribution depends on $\sigma_g$
    - $z:$ characteristics of nests, $\sigma_g\in[0,1]$ correlation of choices in nest $g$, and $\nu_{ij}\sim$ EV Type-I
- Cluster sets of choices into different nests so choices are correlated inside the nest.
- We force independence across nests.

</div>

---

<!-- .slide: data-transition="slide" -->

### Demand Model

<div style="font-size:25pt;line-height:70px">

<div>
$$\begin{align}
 u_{ij}&=x_j\color{purple}{\beta_i}+\xi_j-\alpha p_j+\epsilon_{ij}\\
        &=x_j\color{purple}{\sum_{k}\left( \beta_k+\sigma_k\zeta_{ik}\right)}+\xi_j-\alpha p_j+\epsilon_{ij}\\
        &=x_j\beta+\color{red}{\sum_{k}\left( x_j\sigma_k\zeta_{ik}\right)}+\xi_j-\alpha p_j+\epsilon_{ij}\\
        &=\color{blue}{x_j\beta}+\color{red}{\nu_{ij}} \ \color{blue}{+\xi_j-\alpha p_j}+\epsilon_{ij}\\[5px]
        &\text{ where } \nu_{ij}\sim G(x,\sigma) \text{: distribution of individuals}.
\end{align}$$
</div>

<div style="margin-bottom:2cm;"></div>
<div style="text-align: left;">

Then we define **mean utility** $\delta_j\equiv x_j\beta-\alpha p_j+\xi_j$,

and rewrite: $u_{ij}=\color{blue}{\delta_j}+v_{ij}+\epsilon_{ij}$.

</div>
</div>

---

# Nest Fixed Point Algorithm

Finding $ \ \xi_j(\theta) \ $ and $ \ \theta$

-v-

<!-- .slide: data-transition="slide" -->
#### Inner Loop: find the fixed point of $ \ \xi_j(\theta)$

<div style="font-size:25pt; text-align: left; padding-left:5cm">

1. Fix $\theta=\big( \alpha, \beta, \sigma\big)$
2. Starting from arbitrary $\delta_j^0(\theta)$, then iterate the contraction:

</div>

<div style="font-size:25pt;">

<div>
$$\begin{align}
  \delta_j^{n}(\theta)&=\delta_j^{n-1}(\theta)+\log s_j-\log\bigg[ {\text{S}}_j\Big(\delta_j^{n-1}(\theta), \theta\Big)^{R}\bigg]\\
  \text{untill } &\Big|\Big|\delta_j^n(\theta)-\delta_j^{n-1}(\theta)\Big|\Big|<10^{-14}\Longrightarrow \text{obtain }\delta_j^*(\theta)
\end{align}$$
</div>

</div>

-v-

#### Outer Loop: recover $\theta$

<div style="font-size:25pt;">

1. Plug $\xi_j(\theta)$ back to the GMM estimator:

    $$\widehat{\theta_{\text{GMM}}}=\underset{\theta}{\arg\min} \Big( \xi_j(\theta)Z\Big)'\widehat{\Omega}^{-1}\Big( \xi_j(\theta)Z\Big)$$

2. Implement 2-step GMM to back out $\theta$

</div>

<script src="plugin/math/math.js"></script>
<script>
  Reveal.initialize({ plugins: [ RevealMath.KaTeX ] });
</script>