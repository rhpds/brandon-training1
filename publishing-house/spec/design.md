# Showroom Lab Authoring Essentials

<!-- This file is the design document for your lab or demo. -->
<!-- Fill in each section below, or run /rhdp-publishing-house to have the intake skill help. -->
<!-- Sections marked with [brackets] are placeholders — replace with real content. -->
<!-- The validation gate checks for all required sections before submission. -->

## Overview

This lab teaches new Showroom lab authors how to write and configure labs using the Publishing House framework. Participants learn AsciiDoc syntax, Antora documentation site configuration, and UI tab setup through hands-on exercises. By the end, authors can create new Showroom labs from scratch, configure navigation, and set up terminal and external link tabs for learner environments.

## Target Audience

- **Role:** Lab authors, content developers, technical trainers
- **Experience level:** Beginner
- **What they already know:** Basic familiarity with YAML syntax and markup languages
- **What they don't know:** AsciiDoc-specific syntax, Antora site structure, Showroom UI configuration

## Prerequisites

- Basic understanding of YAML configuration files
- Text editor experience
- No hands-on experience required; all work is browser-based editing and reading configuration files

Can prerequisites be auto-verified? No — this is a training lab with no automated environment checks.

## Learning Objectives

1. Configure AsciiDoc variables in site.yml and use the Antora image macro to insert images into lab content
2. Understand and configure Antora component descriptors, navigation files (nav.adoc), and the module hierarchy for documentation structure
3. Configure terminal and external link tabs in Showroom UI environments using tab properties and validation

## Content Type

Lab (hands-on)

## Products & Technologies

- AsciiDoc (documentation markup language)
- Antora (documentation site builder and content management system)
- YAML (configuration file format)

## Module Map

| Module | Title | Duration |
|--------|-------|----------|
| 1 | Writing your lab | 10 min |
| 2 | Antora | 10 min |
| 3 | Tabs | 10 min |
| — | **Total hands-on** | **0.5 hours** |
| — | **Total lab** | **~0.5 hours** |

## Difficulty Level

Beginner

## Environment

**Learner view:** Participants see a browser window with Showroom documentation pages and lab configuration files open in a text editor. They view AsciiDoc source files, YAML configuration examples, and rendered HTML output side-by-side.

**Automation needed:** No — this is a knowledge transfer lab with no infrastructure or automation requirements.

## Infrastructure Requirements

- **Cloud provider:** Not applicable
- **Cluster type:** Not applicable
- **OCP version:** Not applicable
- **Topology:** Not applicable
- **Sizing:** Not applicable — no infrastructure needed
- **Automation approach:** None (all content is browser-based editing and configuration review)
- **AI/MaaS:** None
- **External services:** AsciiDoc documentation site (docs.asciidoctor.org) for reference; no backend infrastructure required
- **AAP version:** Not applicable
- **Non-GA products:** None (all products are GA)

## Assessment Strategy (Optional)

Assessment is implicit: participants successfully complete each module when they understand the configuration concepts and can explain the purpose of each configuration element. No automated verification is required. Success indicators are:
- Module 1: Participant can identify correct AsciiDoc syntax for variables and image macros
- Module 2: Participant can map Antora YAML keys to navigation output
- Module 3: Participant can explain tab type differences and configure a tab property
