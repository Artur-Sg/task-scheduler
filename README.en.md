[🇷🇺 Русский](README.md) | 🇬🇧 English

# Task Scheduler

A runtime-agnostic task scheduling library with support for priorities, delayed execution, cooperative task execution, cancellation, and pluggable executors.

## Motivation

Modern applications regularly perform computationally expensive operations:

* filtering large datasets;
* processing files;
* computing derived data;
* analyzing and transforming data structures;
* handling user input in the background.

Executing such workloads without an explicit scheduling strategy may block the main execution thread and reduce application responsiveness.

## Project Goal

The goal of this project is to explore and implement a universal scheduling model for computational work, providing control over the order, priority, and execution strategy of tasks.

Task management is achieved through:

* priority-based scheduling;
* delayed execution;
* cooperative execution of long-running tasks;
* task cancellation;
* pluggable executors;
* offloading heavy work to external executors, such as worker pools.

## Primary Use Cases

### Large Dataset Search

Users can continue typing while data filtering is being performed in the background.

### File Import

Large files can be processed asynchronously and the operation may be cancelled by the user.

### Derived Data Computation

Background computations should not interfere with user interactions.

### Heavy Work Offloading

Computationally intensive workloads can be delegated to external executors to avoid blocking the main application.

## Current Status

🚧 The project is currently in the design phase.

The current focus includes:

* terminology;
* execution model;
* task lifecycle;
* cancellation semantics;
* priority system;
* executor architecture.

## Documentation

* Vision
* Terminology
* Execution Model
* Architecture
* Roadmap
