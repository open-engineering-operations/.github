# Open Engineering Operations

The operational layer for the Open Engineering Ecosystem.

![Open Engineering Operations hero-banner.png](../assets/hero-banner.png)

Open Engineering Operations provides the interfaces, workflows and automation required to observe, operate and evolve an Open Engineering ecosystem.

OE defines the engineering truth. Operations makes that truth actionable.

⸻

What we build

Open Engineering Operations connects humans, AI workers and Open Engineering components through a common operational layer.

                 Open Engineering Ecosystem
                            │
                  ┌─────────▼─────────┐
                  │   Definitions     │
                  │   Models & Rules  │
                  └─────────┬─────────┘
                            │
                  ┌─────────▼─────────┐
                  │ Picos & Capsules  │
                  └─────────┬─────────┘
                            │
             ┌──────────────┼──────────────┐
             │              │              │
           APIs           Events        Telemetry
             │              │              │
             └──────────────┼──────────────┘
                            │
                  ┌─────────▼─────────┐
                  │    Operations     │
                  │                   │
                  │ Observe           │
                  │ Operate           │
                  │ Review            │
                  │ Automate          │
                  └───────────────────┘

Our focus includes:

* operational dashboards;
* Pico and Capsule lifecycle management;
* health and telemetry;
* workflow orchestration;
* human-in-the-loop operations;
* AI worker management;
* memo implementation workflows;
* approvals and escalations;
* operational APIs and events;
* deployment and runtime operations.

⸻

Human + AI Operations

Open Engineering Operations is designed for an ecosystem where software is developed and operated by a combination of humans and AI workers.

A typical workflow can look like:

             Specification
                   │
                   ▼
                memo.md
                   │
                   ▼
             Human Review
                   │
                   ▼
             AI Worker Pool
             ┌─────┴─────┐
             │           │
          Local LLM    Cloud LLM
             │           │
             └─────┬─────┘
                   │
                   ▼
              Implementation
                   │
                   ▼
                Validation
                   │
             ┌─────┴─────┐
             │           │
           PASS         FAIL
             │           │
             ▼           ▼
          Complete    Escalation
                         │
                         ▼
                   Human Review

The Operations layer makes this process visible and actionable.

⸻

Operational interfaces

We favour replaceable operational interfaces rather than coupling the ecosystem to a single UI technology.

Possible interfaces include:

* web applications;
* command-line tools;
* dashboards;
* AI agents;
* MCP integrations;
* automation platforms;
* low-code operational applications.

For example, Budibase can be used as a self-hosted operational interface for dashboards, forms and workflows.

The important architectural principle is:

The interface operates Open Engineering; it does not become Open Engineering.

⸻

Architecture

Open Engineering Operations follows a separation of concerns:

Canonical OE definitions
          │
          ▼
      OE services
          │
          ├── APIs
          ├── Events
          └── Telemetry
                    │
                    ▼
             Operations layer
                    │
          ┌─────────┼─────────┐
          ▼         ▼         ▼
        Human      AI       Automation
        UI        Agents      Workers

This keeps operational tooling replaceable while preserving the canonical Open Engineering model.

⸻

Repositories

This organisation contains projects supporting the operational side of the Open Engineering Ecosystem.

Projects may cover:

* Operations;
* operational APIs;
* workflow automation;
* telemetry;
* human review;
* AI worker orchestration;
* deployment;
* operational dashboards;
* integrations.

See individual repositories for their current status, architecture and implementation details.

⸻

Open Engineering

Open Engineering Operations is part of the wider Open Engineering Ecosystem.

Open Engineering is based on a simple idea:

Element-Oriented Engineering automates the Envelope, preserves the Letter, and continuously grows the Library.

Operations provides the mechanisms through which that ecosystem can be observed, controlled and continuously improved.

⸻

Status

🚧 Actively evolving

The ecosystem is being developed incrementally through experiments, prototypes, architectural decisions and implementation memos.

We favour:

small experiments → explicit decisions → reusable components → continuous evolution

⸻

Contributing

Contributions, experiments and ideas are welcome.

Before implementing a substantial change, please consider documenting the intended change as a memo.md so that the reasoning remains part of the engineering history.

⸻

Open Engineering Operations

Observe. Operate. Evolve.
