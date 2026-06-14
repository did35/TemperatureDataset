# Temperature Dataset Analysis

## Objective

Investigate whether modern temperature records show
evidence of acceleration or deceleration by using
first and second derivative analysis.

## Methodology

1. Collect temperature datasets
2. Apply moving averages
3. Calculate first derivative (rate of change)
4. Calculate second derivative (acceleration)
5. Compare historical and modern periods

## Datasets

### Berkeley Earth
### HadCRUT
### CET
### UAH (optional)

## Limitations

- Dataset uncertainty
- Choice of smoothing window
- Regional versus global datasets
- Derivative sensitivity to noise

## Future Work

- FastAI forecasting experiments
- Comparison with ENSO indices
- Volcanic forcing analysis
- Solar activity analysis

# Temperature Dataset

## 1. Berkeley Earth Dataset

<img width="1800" height="1012" alt="Global Land-temperature-chart" src="https://github.com/user-attachments/assets/125f32be-db42-4f05-abc0-4aee523e6c12" />


[Berkeley Earth Global Land Temperature](https://berkeley-earth-temperature.s3.us-west-1.amazonaws.com/Regional/TAVG/global-land-TAVG-Trend.txt)

---

## 2. CET comparaison

<img width="3000" height="1800" alt="CET" src="https://github.com/user-attachments/assets/1e4e020a-df2e-4f76-84a2-dbde7dbbe152" />


[CET 1659 - 2025](https://www.metoffice.gov.uk/hadobs/hadcet/graphs/ts_meantemp_cet.png)

---

## 3. Historical Events

[Maunder Minimum 1645 - 1715](https://en.wikipedia.org/wiki/Maunder_Minimum)

[Dalton Minimum 1790 - 1830](https://en.wikipedia.org/wiki/Dalton_Minimum)

[Capture of the Dutch Fleet - 1795](https://www.youtube.com/watch?v=-9oGZKscpe8)

[Napoleon's Retreat from Moscow - 1812](https://www.youtube.com/watch?v=lNReCCShKJQ)

---

# Calculus Refresher

## 4. Slope, Derivative, and Acceleration: A Refresher

## Overview

A derivative measures how fast something changes.

Examples:

- Position → Velocity
- Velocity → Acceleration
- Temperature → Warming rate
- Warming rate → Acceleration of warming

---

## a. Slope

Consider a function (replace program by function):

<img width="794" height="180" alt="Graph function" src="https://github.com/user-attachments/assets/2d54dfa4-8814-4e58-8ee3-e87566eb2f0b" />

```
y = f(x)
```

The slope tells us how steep the curve is at a given point.

### Average slope

Between two points:

```
Δy / Δx
```

Example:

```
(20 - 10) / (5 - 0) = 2
```

The function increases by 2 units for every 1 unit of x.

---

## b. Derivative

The derivative is the instantaneous slope.

Instead of measuring over an interval, we measure the slope at a single point.

Notation:

```
f'(x)
```
Lagrange notation

or

```
df/dx
```
Leibniz notation

### Interpretation

| Derivative | Meaning |
|------------|----------|
| f'(x) > 0 | Function increasing |
| f'(x) < 0 | Function decreasing |
| f'(x) = 0 | Flat point (possible maximum or minimum) |

---

## c. Motion Example

### Position

s(t)

Position as a function of time.

Example:

- 0 m
- 10 m
- 20 m
- 30 m

---

### Velocity

Velocity is the first derivative of position.

v(t) = ds/dt

Meaning:

Velocity tells us how quickly position changes.

Units:

m/s

---

### Acceleration

Acceleration is the derivative of velocity.

a(t) = dv/dt

Acceleration is also the second derivative of position.

a(t) = d²s/dt²

Meaning:

Acceleration tells us how quickly velocity changes.

Units:

m/s²

---

## d. Calculus Chain

Position
↓ derivative

Velocity
↓ derivative

Acceleration

Written as:

s(t) → v(t) → a(t)

or

s(t) → s'(t) → s''(t)

---

## e. Reverse Process

Integration reverses differentiation.

Acceleration
↑ integration

Velocity
↑ integration

Position

Written as:

a(t) → v(t) → s(t)

---

## f. Climate Data Interpretation

Suppose:

T(t)

represents a temperature anomaly dataset.

### First Derivative

T'(t)

Measures the warming rate.

Interpretation:

- Positive → warming
- Negative → cooling

---

### Second Derivative

T''(t)

Measures the acceleration of warming.

Interpretation:

| Second Derivative | Meaning |
|------------------|----------|
| T''(t) > 0 | Warming accelerating |
| T''(t) = 0 | Constant warming rate |
| T''(t) < 0 | Warming still occurring but slowing |

---

## Aviation Analogy

Altitude = Position

Vertical Speed = First Derivative

Acceleration = Second Derivative

Example:

- Climbing at 1000 ft/min → positive first derivative
- Increasing from 1000 to 2000 ft/min → positive second derivative
- Reducing from 2000 to 1000 ft/min → negative second derivative

---

## Why This Matters

Looking only at the data:

"Is it increasing?"

uses the first derivative.

Looking deeper:

"Is the increase itself speeding up or slowing down?"

uses the second derivative.

This is why derivatives are powerful tools for studying:

- Physics
- Engineering
- Economics
- Climate datasets
- Machine Learning
- Deep Learning (Gradient Descent)

---

## What this project is NOT

This project is not intended to prove or disprove
anthropogenic climate change.

Its purpose is to explore temperature datasets
using basic mathematical tools that can be
understood by anyone with high-school level calculus.

The first derivative tells us how fast something changes.

The second derivative tells us whether that change is speeding up or slowing down.
