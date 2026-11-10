# Conformance Reboot 2027

> **Status:** Tentative proposal for Conformance Work Group feedback. Publishing
> this draft starts the review; it does not approve the content. This is not a
> published standard, an HL7 ballot, or a final decision.

The HL7 Conformance Work Group needs to reboot and restart its engagement with
the community. The proposed approach is research first: learn current
conformance practice across FHIR implementation guides, organize the group's
work in InteropHub, and then, when the homework supports it, offer voluntary
workshops to guide authors. This repository gathers what has been proposed so
far so the group can review and improve it.

This repository is the Topic Reference for
[Conformance Reboot 2027, InteropHub topic 146](https://informatics.immregistries.org/hub/es/topic/146). It records where
the topic currently stands: its definitions, principles, diagrams, working
decisions, and open questions.

## Start here

1. Read the [Topic Reference](https://nathanbunker.github.io/conformance-reboot-2027/latest/), where you can also leave
   comments, or the [GitHub reading copy](CoreDocument.md), or browse the
   [canonical source sections](content/README.md).
2. See the [working decisions and open questions](content/90-working-decisions.md).
3. Read [how to contribute](CONTRIBUTING.md).

## What belongs here, and what does not

This project covers the reboot itself: why it is needed, its proposed mission
and principles, the named parts of the work, roles, measures of progress, and
the group's working decisions and open questions. Substantive conformance
findings, research tooling design, and the Core Intent and acknowledgment work
belong to separate topics or projects; see
[Status and Scope](content/00-status-and-scope.md).

This repository is hosted on a maintainer's personal GitHub account for now,
because the work belongs to the HL7 Conformance Work Group rather than to the
organization that hosts most other Topic References.

## Community coordination

The community works on this topic through InteropHub:
[Conformance Reboot 2027, topic 146](https://informatics.immregistries.org/hub/es/topic/146). Meetings, agendas, and
discussion notes are tracked there.

## Build

Initialize the shared templates after cloning:

```powershell
git submodule update --init
```

Build the reading copy, Word and HTML review copies, and the web guide in
`output/`:

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File .\build.ps1
```

Validate source and generated files:

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File .\validate.ps1
```

Pushing to `main` publishes the guide at https://nathanbunker.github.io/conformance-reboot-2027/main/. Pushing a release
tag such as `v0.1.0` publishes it at that version and at
https://nathanbunker.github.io/conformance-reboot-2027/latest/.

## Repository structure

```text
content/            canonical Markdown for the core document
products/           derived products, including the web guide
review/             review inputs awaiting adjudication
sources/            list of source material and how it is used
process/            submodule: shared public templates and tools
output/             generated files; not committed
ConformanceReboot2027.qmd    assembly authority for section order
CoreDocument.md     generated single-file reading copy
guide.json          web guide settings
```
