---
layout: post
title: "5S for Software Teams"
subtitle: "Random thought about how does one goes about implementing 5S metthodology in Softwware Developement Environment"
date: 2026-02-13 12:00:00 -0500
tags: [5S, agile, engineering, lean, jira, repository-management]
categories: [engineering, process]
comments: true
excerpt: "Apply the Toyota 5S methodology to engineering repositories and JIRA boards for sustainable velocity and team clarity."
---

*In my early days of my career, I had an oppotunity to intern at a Japanese factory, where I first hand saw various lean methodlogies and techniques applied, and one of the things that inspired me was 5S Inspired by the 5S methodology from the Toyota Production System.*

What is 5S ?
5S is a lean manufacturing methodology for organizing, cleaning, and maintaining a productive, safe work environment. It uses five Japanese pillars: Seiri (Sort), Seiton (Set in Order), Seiso (Shine), Seiketsu (Standardize), and Shitsuke (Sustain). By creating a "place for everything," it reduces waste, improves efficiency, and boosts morale.
---

## Why 5S for Software?

Modern software teams suffer from invisible clutter:
- Bloated repositories
- Stale branches
- Unclear ownership
- Massive backlogs
- Misleading metrics

5S brings operational discipline to:
- Code repositories
- JIRA boards
- Agile execution systems

The goal is **flow, clarity, and sustainability**.

---

## The 5S Framework Applied to Software

| 5S Principle | Meaning | Software Interpretation |
|--------------|----------|-------------------------|
| **Seiri (Sort)** | Remove unnecessary items | Eliminate dead code, stale tickets, unused branches |
| **Seiton (Set in Order)** | Organize for flow | Logical repo structure, clear workflows |
| **Seiso (Shine)** | Clean and inspect | Refactor, review, inspect boards regularly |
| **Seiketsu (Standardize)** | Make standards visible | Templates, branch rules, workflow consistency |
| **Shitsuke (Sustain)** | Discipline and culture | Continuous enforcement and leadership alignment |

---

## 1️⃣ Seiri — SORT

### Objective
Remove waste from both engineering artifacts and workflow systems, below is a sample list of areas, and actions, teams have to decide the cadence and ownership based on their code churn

| Area | Actions | 
|------|----------|
| **Code Repository** | Remove dead code |
| | Delete stale branches (>30 days inactive) | 
| | Archive deprecated modules | 
| | Remove unused dependencies | 
| **JIRA** | Close stale tickets (>90 days no update) | 
| | Merge duplicate stories |
| | Move unclear ideas to Parking Lot | 
| | Remove "Zombie Epics" | Quarterly | 

---

## 2️⃣ Seiton — SET IN ORDER

### Objective
Everything has a place. Navigation should be intuitive.

| Area | Standards | Enforcement Method |
|------|-----------|-------------------|
| **Code Repository** | Domain-based folder structure | Architecture guidelines |
| | Branch naming: `feature/`, `bugfix/`, `hotfix/` | Git hooks / PR checks |
| | README with setup instructions | PR checklist |
| | Separate infra, app, and test layers | Code review |
| **JIRA** | Clear workflow states (To Do → In Progress → Review → Done) | Workflow configuration |
| | Definition of Ready | Refinement ceremony |
| | Definition of Done | Sprint review gate |
| | Consistent ticket template | Required fields |

---

## 3️⃣ Seiso — SHINE

### Objective
Clean continuously and inspect frequently.

| Area | Inspection Mechanism | Trigger |
|------|----------------------|---------|
| **Code Repository** | Code reviews | Every PR |
| | Static analysis & linting | CI pipeline |
| | Test coverage reports | Every build |
| | Refactoring backlog | Sprint capacity allocation |
| **JIRA** | Backlog grooming | Weekly |
| | WIP review | Daily stand-up |
| | Cycle time monitoring | Sprint review |
| | Blocked ticket audit | Twice weekly |

---

## 4️⃣ Seiketsu — STANDARDIZE

### Objective
Make the correct behavior the default behavior.

| Area | Standard | Tooling |
|------|----------|---------|
| **Code Repository** | PR template enforced | GitHub settings |
| | Commit message convention | Commit lint |
| | Automated testing required | Branch protection rules |
| | Code formatting auto-enforced | Pre-commit hooks |
| **JIRA** | Mandatory acceptance criteria | Required custom fields |
| | Story size limits | Estimation policy |
| | WIP limits | Kanban configuration |
| | Epic breakdown standard | Product governance |

---

## 5️⃣ Shitsuke — SUSTAIN

### Objective
Build discipline into team culture.

| Area | Cultural Practice | Leadership Responsibility |
|------|-------------------|---------------------------|
| **Code Repository** | No "temporary hacks" | Protect engineering time |
| | Refactor within feature work | Capacity allocation |
| | Rotate code ownership | Knowledge sharing |
| **JIRA** | Do not overload sprint | Enforce velocity realism |
| | Finish before starting | Protect WIP limits |
| | Metrics guide decisions | Review flow data monthly |

---

## Metrics to Track

| Metric | Healthy Signal | Warning Sign |
|--------|---------------|--------------|
| Lead Time | Stable and predictable | Increasing variance |
| WIP | Within limits | Constant overload |
| PR Size | Small and reviewable | Massive change sets |
| Open Tickets | Controlled backlog | 500+ aging items |
| Test Stability | <2% flaky | Frequent reruns |

---

## Anti-Patterns to Avoid

- Treating JIRA as a storage system
- Using long-lived branches
- Skipping code reviews under deadline pressure
- Overloading sprint capacity
- Measuring utilization instead of flow

---

## What "Good" Looks Like

- Clean commit history
- Small, meaningful PRs
- Predictable sprint delivery
- Minimal blocked tickets
- Fast CI
- Engineers confident modifying any area of code

---

## Final Principle

> A messy system produces messy outcomes.  
> A disciplined system produces sustainable velocity.

5S is not about perfection. It embodies a continuous improvement principle
It is about reducing waste so teams can focus on delivering value.

---
