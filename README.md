# Reliance Lens

## Different technologies do not necessarily mean different exposure.

Technically different approaches can look diversified while still relying on the same people, infrastructure, resource, process, environmental condition, or recovery capability.

That creates a strategic question:

> **When we choose between different technologies, are we actually reducing exposure—or only changing the mechanism?**

**Reliance Lens** is a comparative instrument for investigating that question.

---

## The idea

Most technology comparisons start with difference:

* What is the architecture?
* How does the mechanism work?
* What does it cost?
* How does performance compare?

Reliance Lens starts one level higher:

> **What must work for each approach to deliver the intended outcome?**

It then asks whether those requirements converge.

The comparison is:

**Approach → Function → Reliance → Coupling → Independence**

### Approach

What makes the systems technically different?

### Function

What common real-world job must they perform?

### Reliance

What specific condition, capability, resource, infrastructure, process, specialist function, or recovery pathway does each require?

### Coupling

Where do those reliances converge?

### Independence

If one approach is disrupted, scarce, constrained, or scaled, does choosing another actually reduce the relevant exposure?

---

## Why this matters

Technical diversity is not necessarily operational independence.

Two systems can use different mechanisms while depending on the same underlying capability.

Conversely, two systems may appear to share a reliance while actually drawing on different resources or recovery pathways.

So the important finding is not:

> “These technologies have a common dependency.”

It is:

> **“Choosing between these technologies does—or does not—separate the exposure that matters.”**

That distinction is the point of the Lens.

---

## Example: brain-computer interfaces

Consider different neural-interface architectures.

They differ in how signals are acquired, in invasiveness, channel characteristics, decoding approaches, and other technical dimensions.

Reliance Lens asks a different question:

> **What must remain true for useful neural-to-action control to remain usable over time?**

One candidate shared reliance is the ability to maintain a usable control loop as biological, behavioral, decoder, and device conditions change.

That does **not** establish a common bottleneck or common risk.

The approaches may differ substantially in the recovery capability they require.

The test is therefore empirical:

* intervention frequency
* recalibration frequency
* performance drift
* restoration time
* independent-use rate

The question is whether those requirements actually converge enough to create meaningful shared exposure.

---

## Example: warehouse automation

Consider:

* autonomous mobile robots
* fixed robotic picking
* human picking supported by software

Their mechanisms differ.

But all must recover when inventory, equipment, routes, objects, or human activity depart from the expected state.

A candidate shared reliance is:

> **sufficient recovery capacity when the nominal operating state breaks down.**

The relevant question is not whether all three “need humans.”

It is whether they rely on the **same scarce recovery capability**.

Useful evidence might include:

* intervention rate
* recovery time
* autonomous-resolution rate
* takeover burden
* lost throughput
* recovery-capacity utilisation

If the recovery pathways are materially different, the apparent shared exposure may disappear.

---

## What this is

**Reliance Lens is:**

* a comparative instrument
* a way to examine operational reliance beneath technical difference
* a method for testing whether apparent technological diversity creates genuine independence
* a hypothesis-generation and stress-testing aid

It is not:

* a technology-ranking system
* a generic AI framework
* a replacement for technical diligence
* proof that different technologies share the same exposure
* proof that a shared reliance is material
* a system for automatically discovering hidden risks

The Lens is deliberately designed to allow the answer to be:

**“There is no meaningful shared exposure.”**

That is a valid result.

---

## Evidence standard

The Lens separates three things:

**Observation**
What is known about an approach and its operating requirements.

**Inference**
What appears to be shared across approaches.

**Test**
What evidence could support or overturn that inference.

The objective is not to produce a compelling story about convergence.

It is to determine whether the convergence survives scrutiny.

---

## Cross-domain stress tests

The framework is being tested across domains where the mechanisms, operating environments, and failure modes differ substantially:

* [BCI](./evidence/bci.md)
* [Warehouse automation](./evidence/warehouse-automation.md)
* [Water treatment](./evidence/water-treatment.md)

These are tests, not claims of universal validity.

Each asks whether the Lens produces a useful distinction between **technical difference** and **operational independence**.

---

## Status

**Reliance Lens is an experimental analytical instrument.**

The implementation is intentionally small.

The proposition is deliberately narrow:

> **Technological diversity may provide less independence than it appears to when different approaches remain coupled through shared operational reliance.**

The useful question is therefore not simply:

> **How different are these technologies?**

It is:

> **Does choosing differently actually separate the exposure?**

## Try the instrument

**[Open Reliance Lens](https://gmuthoni.github.io/reliance-lens/)**

## Stress tests

* [BCI](evidence/bci.md)
* [Warehouse automation](evidence/warehouse-automation.md)
* [Water treatment](evidence/water-treatment.md)
