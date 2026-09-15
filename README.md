# Jesse Williamson — Technical Portfolio

Senior Technical Support Engineer focused on enterprise software, applied AI, cloud infrastructure, systems integration, and technical systems that interact with the physical world.

My background combines chemical engineering, enterprise software, customer-facing technical work, and hands-on software development. I am especially interested in problems where software, data, AI, and real-world operations intersect.

This portfolio highlights selected completed and in-progress work across scientific machine learning, retrieval systems, and enterprise automation.

---

# Featured Project

## Physics-Informed Neural Network Framework for Engineering Systems

### Overview

A modular PyTorch framework for solving engineering systems using physics-informed neural networks.

The project explores how neural networks can incorporate governing differential equations directly into training while still being validated against established numerical methods.

The long-term goal is to create a reusable framework that can move beyond a single reference problem toward parameterized engineering models and broader process-system applications.

### Why I Built It

Traditional engineering models rely heavily on numerical solvers and specialized simulation software.

I wanted to explore whether physics-informed neural networks could provide another way to model engineering systems while preserving:

- Physical consistency
- Validation against trusted numerical methods
- Reproducibility
- Modularity
- Extensibility to new engineering problems

The project also gave me an opportunity to combine my chemical engineering background with Python, PyTorch, numerical methods, and software architecture.

### Current Implementation

The framework currently includes:

- A reference plug flow reactor model
- Governing differential equations embedded directly into the training loss
- Automated validation against SciPy numerical solvers
- Unit testing
- Configuration-driven training
- Model checkpointing
- GPU-accelerated PyTorch training
- Reusable model and evaluation components
- Structured validation workflows
- Architecture designed to support parameterized engineering models

The reference implementation has been validated against a conventional numerical solution and is being used as the baseline for a parameterized version of the model.

### Technical Architecture

```text
Engineering Problem Definition
        ↓
Physical Parameters + Boundary Conditions
        ↓
Neural Network
        ↓
Predicted Engineering State
        ↓
Automatic Differentiation
        ↓
Physics Residuals
        ↓
Physics-Informed Loss
        ↓
Training
        ↓
Validation Against Numerical Solver
