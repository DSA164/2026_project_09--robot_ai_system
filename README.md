# 2026 Project 10 — Robot AI System

## Purpose

This project is part of the `AI-Engineering-Lab` learning roadmap.

It applies AI engineering concepts to robotics. The goal is to connect perception, local inference, decision logic, and safe control in a small robot-oriented system.

This project should distinguish clearly between AI assistance and deterministic safety-critical control.

## Why this project exists

A robot system is not just an LLM connected to motors. It needs a controlled loop:

```text
sensor
  ↓
perception
  ↓
state estimation
  ↓
decision logic
  ↓
control command
  ↓
motor / actuator
  ↓
feedback
```

This project teaches where AI can help and where deterministic engineering rules are required.

## Learning focus

This project focuses on:

- robot architecture;
- sensors;
- perception;
- local inference;
- command interfaces;
- control loops;
- safety boundaries;
- telemetry;
- feedback;
- hardware-aware constraints.

## Minimal milestone

Create a small prototype where sensor or simulated perception data is converted into a safe high-level decision without directly controlling hardware unsafely.

## Final deliverable

A robot AI prototype with:

- a documented architecture;
- perception or simulated perception input;
- local inference or decision logic;
- a safe command interface;
- logging / telemetry;
- clear safety constraints;
- documented limitations.

## Repository structure

Recommended structure:

```text
hardware/          hardware notes and wiring constraints
notes/             robot architecture and safety notes
src/perception/    sensor or image interpretation
src/control/       safe command logic
src/interface/     operator or API interface
src/telemetry/     logging and state reporting
experiments/       simulation or hardware experiments
MENTORING.md       guided exercises and validation checklist
learning_log.md    session-by-session observations
```

## Success criteria

By the end of this project, I should be able to explain:

- the full chain from sensor to action;
- which parts use AI;
- which parts must remain deterministic;
- how unsafe actions are prevented;
- how feedback is observed;
- how local inference fits into a robot system.

## Relation to the next project

This project prepares `2026_project_11--ai_platform`.

The robot system becomes one possible client of a broader local AI platform with model serving, workflows, RAG, agents, and monitoring.
