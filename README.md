# Temperature Dataset

## Slope, Derivative, and Acceleration: A Refresher

## Overview

A derivative measures how fast something changes.

Examples:

- Position → Velocity
- Velocity → Acceleration
- Temperature → Warming rate
- Warming rate → Acceleration of warming

---

## 1. Slope

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

## 2. Derivative

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

## 3. Motion Example

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

## 4. Calculus Chain

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

## 5. Reverse Process

Integration reverses differentiation.

Acceleration
↑ integration

Velocity
↑ integration

Position

Written as:

a(t) → v(t) → s(t)

---

## 6. Climate Data Interpretation

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

## One-Sentence Summary

The first derivative tells us how fast something changes.

The second derivative tells us whether that change is speeding up or slowing down.
