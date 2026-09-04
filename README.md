# Dependency Lens

## The bottleneck may be one level above the technology.

When technically different approaches are compared, the obvious differences tend to dominate the analysis.

Different architectures.
Different interfaces.
Different business models.
Different technical trade-offs.

But technologies ultimately have to accomplish something in the real world.

That creates a different question:

> **What condition must all of these approaches make work, regardless of how they achieve it?**

Sometimes the important risk is not visible at the level where the technologies differ. It sits one level above them — in a shared dependency.

**Dependency Lens** is a small analytical instrument for finding and testing those dependencies.

---

## The method

The comparison follows five steps:

**Surface → Function → Dependency → Exposure → Test**

### 1. Surface

Start with what makes the approaches appear different.

What architecture, mechanism, interface, or implementation choice separates them?

### 2. Function

Move one level up.

What does each approach actually have to accomplish for the real-world outcome to occur?

This is where apparently different technologies can begin to converge.

### 3. Dependency

Ask what condition must remain true for that function to work.

Examples might include:

* maintaining usable performance as conditions change
* handling exceptions without excessive human intervention
* integrating into an existing workflow
* maintaining calibration or state
* sustaining throughput under variable inputs
* keeping operating or maintenance burden within acceptable limits

These are **candidate dependencies**, not conclusions.

### 4. Exposure

If several approaches depend on the same condition, ask whether that creates meaningful shared exposure.

A common dependency does **not** automatically mean a common bottleneck.

It becomes important when failure, scarcity, cost, maintenance, operational burden, or scaling difficulty at that dependency materially limits the outcome.

### 5. Test

Finally, make the hypothesis vulnerable.

What observable evidence would support it?

And, more importantly:

> **What evidence would make us abandon it?**

A useful dependency should lead to a measurable prediction or a meaningful falsifier.

---

## Why compare technologies this way?

Company-by-company and technology-by-technology analysis is often organized around differentiation.

That makes sense when the question is:

> Which approach is technically better?

It is less useful when the question is:

> **What could still prevent several technically different approaches from succeeding?**

Two architectures can solve a problem differently while still being exposed to the same underlying condition.

That creates a form of concentration that may be invisible in a conventional comparison.

The purpose of Dependency Lens is not to eliminate feature-level analysis.

It is to add another layer.

---

## A simple example

Consider three approaches to warehouse automation:

* autonomous mobile robots
* fixed robotic picking systems
* human-operated picking supported by software

Their architectures are obviously different.

A conventional comparison might focus on:

* throughput
* capital cost
* flexibility
* accuracy
* deployment requirements

Dependency Lens asks a different question:

> **What must all three approaches do when the real operation encounters something the system did not expect?**

That leads to a candidate dependency:

**exception handling and recovery.**

The interesting question then becomes measurable:

> How many human interventions are required per 1,000 tasks, and how long does it take to recover?

The hypothesis could be wrong.

For example, if one architecture demonstrates high throughput with very low intervention requirements across realistic operating conditions, the shared-dependency thesis becomes much weaker.

That is the point.

The method should produce hypotheses that can be rejected, not just patterns that sound insightful.

---

## What this is — and isn't

**Dependency Lens is:**

* a comparison instrument
* a way to move from technological differences to shared operating conditions
* a hypothesis-generation and testing aid
* useful for comparing multiple approaches to the same consequential problem

It can be used by investors, engineers, R&D leaders, clinicians, strategists, acquirers, and others who need to compare technically different approaches.

**It is not:**

* a generic AI framework
* a company-ranking system
* a replacement for technical diligence
* a claim that every technology hides the same bottleneck
* a claim that identifying a dependency proves it is limiting
* a large knowledge-management or organizational-learning platform

The discipline is in knowing when **not** to force a shared dependency.

---

## The key distinction

### Dependency ≠ bottleneck

A dependency is a condition a system relies on.

A bottleneck is a dependency that becomes materially limiting.

That distinction matters.

Finding a shared dependency is only the beginning. The useful analytical question is whether that dependency actually constrains performance, implementation, economics, reliability, or scale.

The final step therefore remains empirical:

**What would we observe if this really were the limiting condition?**

---

## The instrument

The live prototype turns the method into an interactive comparison.

**[Open Dependency Lens →](./index.html)**

The prototype is intentionally lightweight.

It does not pretend to have a hidden database of truth or to automatically discover facts about a market.

Instead, it makes the reasoning structure explicit:

> **Surface → Function → Dependency → Exposure → Test**

The goal is to make a different comparison easier to perform — and easier to challenge.

---

## Cross-domain tests

The method is being stress-tested outside a single technology category.

* [BCI](./evidence/bci.md)
* [Warehouse automation](./evidence/warehouse-automation.md)
* [Water treatment](./evidence/water-treatment.md)

These are not presented as proof that the method is universally valid.

They are attempts to break it.

Each test asks whether the method produces a more useful comparison than simply listing the differences between technologies — and whether the resulting dependency can be stated precisely enough to be falsified.

---

## Intellectual position

The underlying ingredients are not claimed as inventions here.

Functional decomposition, dependency analysis, constraint analysis, systems engineering, technology assessment, bottleneck analysis, and cross-case comparison all have substantial precedents.

The narrower proposition is this:

> **A deliberately cross-architecture comparison, organized around shared function and followed by an explicit falsification step, can expose an important dependency that is easy to miss when each technology is analyzed primarily inside its own vocabulary.**

Whether that proposition is useful is an empirical question.

That is what the tests are for.

---

## Status

**Dependency Lens is an experimental analytical instrument.**

The current implementation is a deliberately small prototype.

The objective is not to build the largest framework.

It is to see whether one sharper question can improve how technically different approaches are compared:

> **What do these technologies have in common that their differences make easy to overlook?**

And then:

> **What evidence would prove us wrong?**
