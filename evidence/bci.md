# BCI

## Problem

Brain-computer interfaces (BCIs) can differ substantially in how they acquire neural signals, how they are implanted, and how those signals are converted into useful control.

The practical problem is broader than any individual interface architecture:

> **Convert neural activity into reliable, useful control for a person under real-world conditions.**

This test asks whether apparently different BCI architectures can be compared by the conditions they must satisfy over time, rather than primarily by the technical features that distinguish them.

---

## Approaches compared

Three broad architectural classes are used for this test:

### Endovascular BCI

A neural interface that reaches target vasculature through an endovascular procedure and records neural activity without requiring direct cortical implantation.

### High-channel-count cortical BCI

A cortical interface designed to record neural activity through a large number of implanted recording channels, with the aim of supporting high-bandwidth decoding.

### Alternative cortical interface

A cortical BCI using a substantially different interface or implantation architecture from conventional high-channel-count approaches.

The purpose is not to determine which architecture is superior.

The purpose is to ask:

> **What must all three approaches accomplish despite how differently they attempt to accomplish it?**

---

## Surface differences

The architectural classes differ along several important dimensions.

| Dimension              | Endovascular BCI                                     | High-channel-count cortical BCI                   | Alternative cortical interface                             |
| ---------------------- | ---------------------------------------------------- | ------------------------------------------------- | ---------------------------------------------------------- |
| Neural access          | Through blood vessels                                | Direct cortical access                            | Direct cortical access using a different interface design  |
| Implantation strategy  | Endovascular                                         | Neurosurgical                                     | Neurosurgical                                              |
| Recording architecture | Distributed neural access through vascular placement | High-density cortical recording                   | Alternative cortical recording approach                    |
| Engineering emphasis   | Access, deployment, signal acquisition               | Recording density, bandwidth, chronic performance | Interface design, recording performance, chronic usability |
| Primary trade-offs     | Access, invasiveness, signal quality, stability      | Bandwidth, implantation, stability                | Interface characteristics, implantation, stability         |

These differences are technically meaningful.

They also create a risk in conventional comparison: the analysis can remain focused on **how the systems differ** without asking what they must all make work after deployment.

Dependency Lens changes the comparison level.

---

## Function

Despite their architectural differences, a useful BCI ultimately has to support a functioning control loop:

**neural activity → signal acquisition → decoding → intended action → user feedback**

The relevant function is therefore not simply:

> “record neural signals.”

It is:

> **Maintain usable neural-to-action control under real-world conditions.**

That function has to persist beyond an initial demonstration.

The system must continue to produce useful control as the user's state, task, neural activity, interface conditions, and decoding environment change.

The architecture determines how the system attempts to perform the function.

It does not remove the requirement to perform it.

---

## Candidate dependencies

Several conditions could plausibly be shared across the architectural classes.

### 1. Technical performance

The interface must acquire neural information with sufficient quality and consistency to support useful decoding.

**Question:** Can the architecture provide sufficiently reliable information for the intended application?

---

### 2. Long-term state maintenance

The system may need to maintain a useful relationship between neural activity and decoded action as biological, behavioral, and technical conditions change.

**Question:** How much recalibration, adaptation, compensation, or intervention is required to preserve useful performance over time?

---

### 3. Workflow integration

The BCI has to function within a broader user and clinical environment.

This may include training, rehabilitation, device configuration, technical support, and specialist involvement.

**Question:** How much external support is required to keep the system usable in practice?

---

## Working hypothesis

### **Long-term state maintenance**

Different BCI architectures may share an underlying dependency:

> **The neural-to-action control loop must remain usable as biological, behavioral, decoder, and device conditions change.**

This is a hypothesis about a **shared dependency**, not a claim that long-term state maintenance is already established as the BCI bottleneck.

The dependency becomes a potential bottleneck only if maintaining usable control materially constrains performance, user independence, cost, scalability, or deployment.

---

## Why this dependency?

The architectural differences determine how neural information is accessed and processed.

They do not necessarily eliminate the need to maintain a usable mapping between:

**neural activity → decoded intent → system action**

This creates an important distinction between:

**initial technical performance**

and

**sustained operational performance.**

A system can demonstrate strong signal quality or decoding performance during a particular period while still requiring substantial intervention to preserve that performance over time.

Conversely, a system that maintains useful control with minimal intervention may have reduced an important operational dependency regardless of its underlying architecture.

The cross-architecture question is therefore:

> **How much work is required to keep the control loop useful?**

If substantially different architectures exhibit similar maintenance requirements, that would support the shared-dependency hypothesis.

If maintenance requirements differ substantially by architecture, the hypothesis becomes weaker.

---

## Decisive evidence

The most useful evidence would measure the operational burden associated with maintaining useful control over time.

Potential measures include:

* specialist interventions per user;
* frequency of decoder recalibration;
* frequency of model adaptation;
* performance degradation between recalibration events;
* time required to restore target performance;
* stability of performance across tasks and sessions;
* proportion of sessions requiring expert adjustment;
* degree of independent use achieved by the user.

A particularly useful measure would be:

> **Specialist intervention required to keep one user at target performance per unit time.**

The direction of the result matters.

If intervention requirements decline substantially as a system matures, that would suggest the dependency is being reduced.

If significant intervention remains necessary across different architectural approaches, the shared dependency becomes more consequential.

The evidence should therefore distinguish between:

> **adaptation exists**

and:

> **adaptation creates a material operational constraint.**

Only the second would support a bottleneck interpretation.

---

## Falsifier

The hypothesis would weaken if an architecture demonstrates:

> **Stable, clinically useful independent control over extended periods with little or no specialist intervention, despite expected changes in biological, behavioral, decoder, and device state.**

It would also weaken if evidence shows that maintenance burden is primarily architecture-specific rather than shared across the different classes.

The existence of recalibration, adaptation, or technical support is therefore not sufficient by itself.

The relevant test is whether:

> **Maintaining usable control becomes a recurring limiting condition across otherwise different BCI architectures.**

If that pattern does not appear, the candidate dependency should be rejected or narrowed.

---

## Judgment

### **PASS — preliminary**

The test produces a plausible cross-architecture dependency:

> **Long-term maintenance of a usable neural-to-action control loop.**

The candidate is useful because it can be translated into observable operational measures rather than remaining a broad statement about “adaptation,” “reliability,” or “integration.”

However, the test does **not** establish that this dependency is the dominant bottleneck for BCIs.

That would require comparative longitudinal evidence across users, systems, and operating conditions.

The appropriate conclusion is therefore:

> **Different BCI architectures may share a dependency that is not obvious from their surface technical differences. That dependency can be investigated through the operational burden required to maintain useful control.**

This is deliberately weaker than claiming that all BCI architectures share the same bottleneck.

---

## What the test exposed about the method

The BCI test suggests that a useful comparison can sit between **technology** and **outcome**.

The analytical sequence is:

**Technology → Function → Dependency → Constraint → Bottleneck**

The important move is not simply finding something that different technologies have in common.

A commonality becomes useful only when it identifies a condition that:

1. multiple approaches must satisfy;
2. can materially affect the outcome;
3. can be observed or measured; and
4. could be shown to be wrong.

The test also exposes a potential failure mode.

Broad concepts such as:

> “adaptation”

> “reliability”

> “integration”

can sound insightful without producing a useful analytical conclusion.

The dependency becomes stronger when the broad concept is translated into a specific operating condition and then into a measurable test.

For example:

**Adaptation**

→ **maintaining a usable neural-to-action mapping as system state changes**

→ **specialist intervention required per user per unit time**

→ **evidence could show that intervention is minimal or architecture-specific**

That progression is the substantive analytical move.

The BCI example therefore does not demonstrate that Dependency Lens discovers hidden bottlenecks.

It demonstrates a narrower proposition:

> **Comparing different architectures through their shared functional requirements can generate a specific dependency that is testable independently of the technologies' surface differences.**

The next domain tests whether that operation remains useful outside BCI.

---

## Sources

The sources below establish the underlying BCI context, including neural interfaces, decoding, clinical development, and long-term operation.

The **shared dependency identified above is an analytical inference**. It is not presented as a conclusion established by any single source.

* Koch, C. et al. (2024). *The road ahead for brain–computer interfaces.* **Nature Electronics.**
  https://doi.org/10.1038/s41928-024-01122-2

* Lebedev, M. A., & Nicolelis, M. A. L. (2017). *Brain-machine interfaces: From basic science to neuroprostheses and neurorehabilitation.* **Physiological Reviews, 97(2)**, 767–837.
  https://doi.org/10.1152/physrev.00027.2016

* Willett, F. R. et al. (2021). *High-performance brain-to-text communication via handwriting.* **Nature, 593**, 249–254.
  https://doi.org/10.1038/s41586-021-03506-2

* Willett, F. R. et al. (2023). *A high-performance speech neuroprosthesis.* **Nature, 620**, 1031–1038.
  https://doi.org/10.1038/s41586-023-06377-x

* Gilja, V. et al. (2012). *A high-performance neural prosthesis enabled by control algorithm design.* **Nature Neuroscience, 15**, 1752–1757.
  https://doi.org/10.1038/nn.3265

* Perge, J. A. et al. (2013). *In vivo stability of a human brain-computer interface.* **Journal of Neural Engineering, 10(3)**, 036021.
  https://doi.org/10.1088/1741-2560/10/3/036021

* Patrick-Krueger, K. M. et al. (2025). *The state of clinical trials of implantable brain–computer interfaces.* **Nature Reviews Bioengineering.**
  https://doi.org/10.1038/s44222-024-00239-5

* Card, N. S. et al. (2026). *Long-term independent use of an intracortical brain-computer interface for speech and cursor control.* **Nature Medicine.**
  https://doi.org/10.1038/s41591-026-04414-6

### Evidence boundary

These sources support facts about BCI technologies, neural decoding, clinical development, and sustained operation.

They do **not** establish that the three architectural classes share a dominant bottleneck.

That proposition remains open to testing.

The purpose of this page is narrower:

> **Identify a candidate dependency at the level of shared function, specify what evidence would support it, and state what evidence would make it weaker.**
