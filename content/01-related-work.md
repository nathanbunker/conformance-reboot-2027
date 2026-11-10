# Related Work

The reboot draws on, and stays separate from, several related efforts. This
section names each one and how it relates to the reboot.

## Related topics

| Topic | Relationship to this work |
|---|---|
| [Conformance Reboot 2027, topic 146](https://informatics.immregistries.org/hub/es/topic/146) | This work. Meetings, agendas, and notes. |

As Reconnaissance produces findings, curated Conformance topics will be added
here.

## FHIR conformance tooling

The Prometheus team expects to investigate tooling that supports FHIR
conformance. The reboot's research helps that work, for example by showing:

- which conformance constructs guides use, and how consistently
- where guides give computable or testable expectations
- where tool support could reduce ambiguity or effort

This interest is **adjacent to the reboot, not part of it**. Taking part in the
research does not mean Conformance endorses a product or a tooling direction.
Author Workshops are not product-validation sessions. Concrete tooling
proposals would go through the appropriate HL7 and community processes.

## IHE testing events and the International Patient Summary

Work at a recent IHE testing event on the International Patient Summary used
Matchbox, an open-source validator built on the HAPI FHIR validator. That
experience raised questions that fit the reboot's interests:

- **Bundle definitions:** how to define what a document bundle must contain
  when its parts can claim different profiles
- **Validator results:** how to read validator output, including whether some
  warnings should be errors
- **Outcome tables:** whether a "truth table" is needed that states what each
  detected issue means for the outcome

These questions are recorded in the topic 146 meeting notes. They are
candidates for curated topics, not conclusions. A European testing event in
April 2027 may also be relevant.

## The HL7 FHIR Community Process

The [FHIR Community Process](https://hl7.org/permalink?FCPRequirements) sets
requirements for organizations, projects, and specifications that publish FHIR
content outside HL7. The requirements cover publication rules, registration,
documentation of quality, and how issues are raised. It is relevant context for
how guides are published and discovered, and for the kinds of conformance
expectations that guides document.

## The Healthcare Interoperability Standards Compliance Handbook

Rob Snelick and Frank Oemig wrote the *Healthcare Interoperability Standards
Compliance Handbook*. It records how they reason about conformance in general,
and could supply concepts, distinctions, and research questions for
Reconnaissance. It does not define FHIR conformance requirements; where its
concepts differ from FHIR, the difference should be stated explicitly. One
idea is to convert a bounded section into a form research agents can use.
This depends on permission and review by the authors.

## Core Intent and acknowledgment behavior

A separate Conformance discussion considers how to define the minimum business
outcome of a transaction, which it calls "Core Intent", and how
acknowledgments should report it, across HL7 v2 and FHIR. It builds on an
acknowledgment management framework that describes how acknowledgment
behavior varies across implementations. It is related work, not part of the
reboot.

## Project intake for InteropHub

A broader idea would use AI-assisted intake to watch public FHIR activity and
propose topics for InteropHub generally. It is future work, to be revisited
once the reboot shows what is worth tracking.
