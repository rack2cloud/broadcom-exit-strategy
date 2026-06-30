# Broadcom Exit Strategy: Migration Architecture Framework
### Control Plane & Execution Physics Transition Model

![Status](https://img.shields.io/badge/status-architectural--framework-blue)

> **Architecture Principle:** Migration is a control-plane and execution-physics transition. Relocating the VMDK is the absolute last layer you should move. 

---
## About This Repository

This repository consolidates the Rack2Cloud research on VMware and Broadcom exit strategy into a structured reference for architects and platform teams.

The Broadcom acquisition of VMware in 2023 forced a re-evaluation of enterprise virtualization strategy across the industry. This repository tracks the architectural dimensions of that transition: licensing economics, platform decision frameworks, migration mechanics, operational continuity, and post-exit failure modes.

The intended audience is architects, platform engineers, and technical leadership responsible for evaluating or executing a VMware exit.

---

## Framework Structure

### Exit Decision Framework

Evaluate whether, when, and how to exit VMware.

**Foundation**

- [The Broadcom Exit Strategy](https://www.rack2cloud.com/post-broadcom-migration-architecture/) — The strategic framing for post-Broadcom architecture decisions.
- [Broadcom Year Two: The Stay or Go Architecture Guide](https://www.rack2cloud.com/broadcom-vmware-fallout-year-two-strategy/) — 2026 decision framework for organizations still evaluating exit timing.
- [The Architecture of Migration: Why Licensing Isn't Your Biggest Risk](https://www.rack2cloud.com/architecture-of-migration-licensing-risk/) — Risk decomposition beyond licensing.

**Legal and Commercial Context**

- [The Broadcom Legal Playbook: Why the VMware Lawsuits Are Accelerating Enterprise Exit Timelines](https://www.rack2cloud.com/broadcom-vmware-lawsuit-legal-playbook/) — Legal pressure as an architectural accelerant.
- [VMware Licensing Costs: Why Most Estimates Are Wrong](https://www.rack2cloud.com/vmware-licensing-costs-estimate/) — Cost estimation failures and how to correct them.
- [March 31 Isn't a Deadline. It's a Forced Architecture Decision.](https://www.rack2cloud.com/vmware-vcsp-termination-architecture-decision/) — VCSP termination as an architectural event (March 2026, now completed).

---

### Platform Evaluation

Compare alternative platforms against VMware across relevant architectural dimensions.

**Decision Frameworks**

- [Nutanix vs VMware: The Post-Broadcom Decision Framework (2026)](https://www.rack2cloud.com/nutanix-vs-vmware-post-broadcom-decision-framework/) — Structured platform comparison for the post-Broadcom environment.
- [Proxmox vs Nutanix vs VMware: The Post-Broadcom Constraints No One Explains](https://www.rack2cloud.com/proxmox-vs-nutanix-vs-vmware-post-broadcom/) — Three-platform constraint analysis.
- [Proxmox Isn't Replacing VMware. It's Replacing Assumptions.](https://www.rack2cloud.com/proxmox-migration-assumptions/) — Why Proxmox evaluations fail when assumptions aren't surfaced first. *(Added 2026-06-30)*
- [Azure VMware Solution vs Native Azure: Architecture Trade-offs, Costs, and Exit Risk](https://www.rack2cloud.com/azure-vmware-solution-vs-native-azure/) — Cloud exit path decision framework for Azure environments.

**Operating Model Considerations**

- [The Hypervisor Is Not the Migration Target — The Operating Model Is](https://www.rack2cloud.com/virtualization-operating-model-migration/) — Why platform selection is the wrong starting point for exit planning. *(Added 2026-06-30)*
- [The VMware Exit Has Entered the Coexistence Era](https://www.rack2cloud.com/vmware-coexistence-era/) — Current state of exit timelines and coexistence patterns.

---

### Pre-Migration Assessment

Assess readiness, dependencies, and risk before migration begins.

**Assessment Framework**

- [VMware Migration Strategy](https://www.rack2cloud.com/modern-virtualization-learning-path/vmware-migration-strategy/) — Strategic migration framework.
- [VMware Licensing Pressure Created a Dependency Audit Problem](https://www.rack2cloud.com/vmware-dependency-audit/) — How licensing pressure created undiscovered dependency exposure. *(Added 2026-06-30)*
- [The Skills Gap Is the Real VMware Exit Risk](https://www.rack2cloud.com/vmware-skills-gap/) — Skills and operational readiness as exit risk factors beyond licensing and platform.

**Assessment Tools**

- [VMware Migration Readiness Assessment](https://www.rack2cloud.com/audits/migration-readiness-assessment/) — Structured pre-migration readiness audit.
- [VMware Licensing Cost Model](https://www.rack2cloud.com/vmware-licensing-cost-model/) — Licensing cost modeling tool.
- [VMware to HCI Migration Advisor](https://www.rack2cloud.com/vmware-to-hci-migration-advisor/) — Migration path decision support tool.

---

### Migration Architecture and Execution

Design and execute the migration with architectural rigor.

**Migration Architecture**

- [Nutanix vs VMware: Availability vs Authority in the Post-Broadcom Datacenter (2026)](https://www.rack2cloud.com/nutanix-vs-vmware-availability-authority/) — Availability and authority as migration design constraints.
- [Performance Modeling the VMware Evacuation: Nutanix AHV vs Proxmox Ceph Storage I/O Reality](https://www.rack2cloud.com/vmware-exit-performance-modeling-ahv-vs-ceph/) — Storage I/O performance modeling for migration planning.
- [The Dashboard Said the Migration Succeeded](https://www.rack2cloud.com/migration-dashboard-failure/) — Why migration validation fails and what to measure instead.

**Execution Patterns**

- [vSphere to AHV Migration Strategy: A Risk-Deterministic Framework for Legacy Workloads](https://www.rack2cloud.com/vsphere-to-ahv-migration-strategy/) — Risk-deterministic framework for legacy workload migration.
- [From vSphere to Nutanix AHV: The Deterministic Migration Checklist to Avoid the 99% Hang](https://www.rack2cloud.com/vsphere-to-nutanix-ahv-migration-checklist/) — Field checklist for AHV migration execution.
- [Migration Stutter: Handling High-I/O Cutovers Without Data Loss](https://www.rack2cloud.com/migration-stutter-high-io-cutover/) — High-I/O cutover design.
- [The Nutanix Migration Stutter: Why AHV Cutovers Freeze High-IO Workloads](https://www.rack2cloud.com/nutanix-migration-stutter-ahv-fix/) — AHV-specific cutover failure analysis.

---

### Post-Exit Operations and Risk

Understand what breaks after the migration and how to design for survivability.

**The Strategic Blueprint:** [Broadcom Exit Strategy: The Post-Broadcom Migration Architecture](https://www.rack2cloud.com/post-broadcom-migration-architecture)

**Post-Exit Failure Modes**

- [Your VMware Exit Was Successful. The First Incident Will Tell You If That's True.](https://www.rack2cloud.com/vmware-exit-survivability/) — Post-exit operational survivability under real incident conditions. *(Added 2026-06-30)*
- [What Breaks First After You Leave VMware](https://www.rack2cloud.com/post-vmware-migration-what-breaks/) — Inventory of post-exit failure modes by category. *(Added 2026-06-30)*

**Operational Architecture**

- [Nutanix AHV Day-2 Operations: The Architectural Reality](https://www.rack2cloud.com/nutanix-ahv-day-2-deep-dive-operations/) — Day-2 operational requirements on AHV post-migration.
- [Nutanix AHV Operations: What Changes After VMware Migration](https://www.rack2cloud.com/nutanix-ahv-operations-after-vmware/) — Operational change inventory for teams transitioning to AHV.
- [Upgrade Physics: Designing for Rolling Maintenance Without Stopping Production](https://www.rack2cloud.com/upgrade-physics-rolling-maintenance-ahv/) — Maintenance architecture for post-migration environments.

---

### Architecture Reference

Supporting architecture content for post-Broadcom infrastructure decisions.

**Virtualization Architecture**

- [Beyond the VMDK: Translating Execution Physics from ESXi to AHV](https://www.rack2cloud.com/beyond-the-vmdk-translating-execution-physics-esxi-ahv/) — Execution physics translation from ESXi to AHV.
- [The CVM Tax: How Mis-Sized Controller VMs Quietly Kill AHV Performance](https://www.rack2cloud.com/cvm-tax-nutanix-ahv-performance/) — AHV controller VM sizing as a post-migration performance constraint.
- [CPU Ready vs. CPU Wait: Why Your Cluster Looks Fine but Feels Slow](https://www.rack2cloud.com/cpu-ready-vs-cpu-wait-why-your-cluster-looks-fine-but-feels-slow/) — Performance modeling for post-migration cluster health.

**Kubernetes as Exit Path**

- [Kubernetes as the VMware Exit Ramp: How Platform Teams Are Reducing VMware Dependence](https://www.rack2cloud.com/kubernetes-vmware-exit-ramp/) — Kubernetes as a parallel exit path.

---

## Canonical Architecture Learning Path

The [Virtualization Architecture Path](https://www.rack2cloud.com/modern-virtualization-learning-path/) provides the structured learning context for this repository's content.

Relevant modules:

- [VMware Migration Strategy](https://www.rack2cloud.com/modern-virtualization-learning-path/vmware-migration-strategy/)
- [Virtualization Control Plane Architecture](https://www.rack2cloud.com/modern-virtualization-learning-path/virtualization-control-plane-architecture/)
- [Virtualization Deterministic Operations](https://www.rack2cloud.com/modern-virtualization-learning-path/virtualization-deterministic-operations/)
- [Virtualization Foundations](https://www.rack2cloud.com/modern-virtualization-learning-path/virtualization-foundations/)

---

## Architecture Audits and Assessments

Structured assessment paths for teams in active exit planning:

- [VMware Migration Readiness Assessment](https://www.rack2cloud.com/audits/migration-readiness-assessment/) — Pre-migration structured assessment.
- [Architecture Audit Services](https://www.rack2cloud.com/audits/) — Full audit service catalog.

---

## Maintenance Notes

This repository is maintained against the Rack2Cloud [Canonical Architecture Specifications](https://www.rack2cloud.com/canonical-architecture-specifications/) governance system.

---

*Last updated: 2026-06-30*
*Maintained by Rack2Cloud — [rack2cloud.com](https://www.rack2cloud.com)*
