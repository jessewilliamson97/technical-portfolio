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
```

### Validation Approach

A major design goal of the project is that the neural-network solution should not simply look reasonable.

The framework validates predictions against conventional numerical methods and tracks error across the full solution profile.

Validation includes:

- Full-profile comparison against SciPy reference solutions
- Conversion error
- Temperature error
- Physics-consistency checks
- Automated unit testing
- Reproducible training configuration

This makes validation part of the framework rather than an afterthought.

### Software Design

The codebase is intentionally structured so that the initial reactor model can serve as a reference implementation rather than becoming tightly coupled to one specific problem.

The architecture separates:

- Physics definitions
- Neural-network architecture
- Loss construction
- Training configuration
- Evaluation
- Validation
- Reusable utilities

The goal is to make it easier to extend the framework to additional engineering equipment and operating domains.

### Current Development Direction

The project is now moving from a fixed-condition reference model toward a parameterized model.

Instead of learning the solution for one set of operating conditions, the parameterized version is intended to learn across an operating domain.

That progression begins to explore the potential value of PINNs as reusable engineering surrogate models rather than one-off numerical experiments.

Longer-term areas of exploration include:

- Additional reactor systems
- Heat exchangers
- Piping systems
- Parameter estimation
- Inverse problems
- Optimization
- Plant-data integration
- Reusable physics-model components

### Technologies

Python  
PyTorch  
SciPy  
NumPy  
PyTest  
GPU Computing  
Automatic Differentiation  
Numerical Methods  
Scientific Machine Learning

### What This Project Demonstrates

This project reflects how I approach technical work:

- Start with a trusted reference solution
- Validate assumptions before adding complexity
- Separate physics from implementation
- Build tests early
- Make experiments reproducible
- Design for extension rather than rewriting
- Use data and validation to guide decisions

---

# Enterprise Retrieval-Augmented Generation System

## Overview

A Python-based prototype for querying large technical document collections using semantic retrieval and LLM-based response generation.

### Problem

Technical organizations often have large repositories of documentation, manuals, engineering references, and internal knowledge that are difficult to search effectively using keyword-based approaches alone.

The goal of this project was to explore how retrieval-augmented generation could improve access to technical information while preserving relevant context for LLM responses.

### What I Built

- Document preprocessing pipelines
- Semantic retrieval
- Vector-based search
- Embedding-based retrieval
- Lexical-versus-semantic retrieval experiments
- Context construction for LLM responses
- Reusable retrieval logic
- Evaluation-oriented experimentation

### Architecture

```text
Technical Documents
        ↓
Preprocessing / Chunking
        ↓
Embedding Generation
        ↓
Vector Index
        ↓
User Query
        ↓
Semantic Retrieval
        ↓
Relevant Context
        ↓
LLM Response
```

### Technologies

Python  
RAG  
Vector Search  
Embeddings  
LLMs  
Semantic Retrieval

### What I Learned

This project strengthened my understanding of:

- Retrieval quality
- Chunking strategy
- Embeddings
- Context construction
- Semantic versus lexical search
- Failure modes in LLM-based systems

---

# Enterprise AI Automation

### In Progress

## Overview

An in-progress Python project exploring how AI-enabled workflows can connect enterprise systems through authenticated APIs.

The project is focused on automation across business systems rather than building an isolated AI demo.

### Current Areas of Development

Current work includes:

- Microsoft Graph integration
- OAuth authentication
- REST API interaction
- Enterprise workflow design
- Salesforce integration
- Modular integration components

### Intended Architecture

```text
User / Business Trigger
        ↓
Python Automation Layer
        ↓
Authentication / OAuth
        ↓
Microsoft Graph
        ↓
Business Logic
        ↓
Salesforce / Enterprise System
        ↓
Result / Follow-Up Action
```

### Current Focus

The project is currently focused on building reliable integration behavior before expanding the automation layer.

Areas being developed include:

- Authentication handling
- API request and response handling
- Failure handling
- Reusable integration components
- End-to-end workflow orchestration
- Logging and observability

### Technologies

Python  
REST APIs  
OAuth  
Microsoft Graph  
Salesforce

### Status

This project is actively under development.

The implementation is not yet complete, so this portfolio describes the current architecture, technical direction, and work completed to date rather than presenting it as a finished system.

---

# Professional Focus

My professional and technical interests sit at the intersection of:

- Enterprise software
- Technical troubleshooting
- Systems integration
- Customer-facing engineering
- Cloud and hybrid infrastructure
- Python
- Applied AI
- Scientific machine learning
- Industrial systems
- Real-world operational problems

I am particularly interested in roles where technical decisions are closely tied to real customer and operational outcomes, including forward-deployed engineering, solutions engineering, technical architecture, and AI infrastructure.

I enjoy technical work where understanding the customer's actual operating problem matters as much as designing the software solution.

---

# About the Code

The primary implementation repositories for these projects are currently private.

This public portfolio provides an overview of the architecture, technical scope, design decisions, validation approach, and development status of selected projects.

Additional technical detail, code samples, architecture discussion, or implementation walkthroughs can be shared during the interview process where appropriate.

---

# Contact

[LinkedIn — Jesse Williamson](https://www.linkedin.com/in/jesse-williamson-eng)
