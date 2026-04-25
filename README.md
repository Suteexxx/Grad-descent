# 🚀 Gradient Descent - Complete Guide

![ML](https://img.shields.io/badge/Machine-Learning-blue)
![Python](https://img.shields.io/badge/Python-NumPy-green)
![Status](https://img.shields.io/badge/Status-Learning-orange)

---

## 📌 What is Gradient Descent?

Gradient Descent is an **optimization algorithm** used to minimize a cost function by updating parameters in the **direction of the negative gradient**.

👉 Simple idea:  
It finds the **best-fit line/model** by reducing error step-by-step.

---

## 📐 Core Formula
θ = θ - α * ∇J(θ)

Where:
- **θ** → Model parameters (m, c)
- **α** → Learning rate
- **∇J(θ)** → Gradient (slope of error)

---

## 📊 Linear Regression Formulation

### Hypothesis
y = mx + c

### Cost Function (MSE)
J(m,c) = (1/n) Σ (y - ŷ)²
