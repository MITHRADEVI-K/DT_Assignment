# The Daily Reflection Tree

### A Deterministic Reflection Agent (No LLM at Runtime)

---

## Overview

This project is a deterministic reflection system designed to guide users through structured end-of-day thinking.

Unlike traditional AI chatbots, this system:

* Does not rely on LLMs at runtime
* Uses a decision tree architecture
* Ensures predictable, auditable, and consistent outputs

The intelligence is embedded in the tree structure, not generated dynamically.

---

## Objective

To build a system that:

* Helps users reflect on their day
* Encourages self-awareness without judgment
* Transforms psychological frameworks into structured decision paths

---

## Core Design

The system is built around a 3-axis psychological model:

### 1. Agency (Locus of Control)

* Internal → “I influenced outcomes”
* External → “Things happened to me”

### 2. Orientation

* Contribution → “What did I give?”
* Entitlement → “What did I deserve?”

### 3. Radius of Concern

* Self → Individual focus
* Team → Group awareness
* Other → Broader impact and purpose

---

## Decision Tree Architecture

* Fully deterministic
* No randomness
* No free-text input
* Every node leads to a predefined next step

Tree Diagram:
![Decision Tree](mermaid-diagram)

---

## Flow Structure

1. Start Node
2. Axis 1: Agency (Locus)
3. Bridge to Axis 2
4. Axis 2: Contribution vs Entitlement
5. Bridge to Axis 3
6. Axis 3: Radius (Self to Others)
7. Summary Generation
8. End

---

## System Components

### Node Types

| Type       | Description                        |
| ---------- | ---------------------------------- |
| start      | Initializes reflection             |
| question   | User selects from fixed options    |
| decision   | Routes based on answers or signals |
| reflection | Provides insight                   |
| bridge     | Transitions between axes           |
| summary    | Final synthesis                    |
| end        | Closes session                     |

---

## State Management

The system tracks:

axis1: { internal, external }
axis2: { contribution, entitlement }
axis3: { self, team, other }

Each answer updates signals like:

axis1:internal += 1
axis2:contribution += 1

---

## Summary Generation

At the end, the system:

* Determines dominant traits across axes
* Generates a personalized reflection summary
* Uses template-based interpolation (no AI generation)

Example:

"You leaned internal on agency and contribution on orientation..."

---

## Key Design Decisions

1. Determinism over AI
   Ensures consistency and avoids hallucination

2. Fixed Options
   Eliminates ambiguity and forces thoughtful design

3. Conversational Flow
   Designed to feel like a dialogue rather than a survey

4. Non-Judgmental Tone
   Encourages reflection without moralizing

---

## Features

* Structured decision tree (25+ nodes)
* Multi-axis psychological mapping
* Dynamic branching logic
* Reflection-based feedback
* Summary generator
* Chatbot-style UI (React)

---

## Tech Stack

Frontend: React.js
State Management: useState
Data Structure: JSON / Tree-based

---

## Example Use Case

A user completes the flow and gains:

* Awareness of their agency level
* Insight into giving versus expecting
* Perspective on self versus others

---

## Future Improvements

* Voice-based interaction
* Progress tracking dashboard
* Deeper adaptive reflection paths
* Mobile-first UI
* User login and session history

---

## About

Mithradevi is a Computer Science student with interests in UI/UX design, product thinking, and building meaningful systems.

The long-term goal is to grow into a servant leader by creating systems that help people think better and improve consistently.

---

## Note

Even though the submission was delayed, this project reflects genuine effort, curiosity, and alignment with the vision of structured, thoughtful systems.

---

Thank you for reviewing.
