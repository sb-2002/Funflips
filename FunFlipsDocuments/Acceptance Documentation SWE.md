---
title: Acceptance Documentation
---

Project: FunFlip Game

Authors:

Ashish Ghaskata\
Krishna Raj Bhandri

Suraj Bhatta

Mohammad Adnan Khan

**Documentname:** AB-Funflip Game-Acceptance Doc

**Version:** 1.0

**Creation date:** 20.06.2025

**File:** \<file location\>

# Table of Contents {#table-of-contents .TOC-Heading .unnumbered}

[**1.** **Introduction** [3](#introduction)](#introduction)[**2.** **SUT
-- System Under Test**
[3](#sut-system-under-test)](#sut-system-under-test)[2.1 System:
[3](#system)](#system)

[2.2 Purpose [3](#purpose)](#purpose)

[2.3 Scope of SUT: [3](#scope-of-sut)](#scope-of-sut)

[2.4 Technology / Architecture:
[3](#technology-architecture)](#technology-architecture)

[2.5 Verification focus : [4](#verification-focus)](#verification-focus)

[**3.** **BZA -- Provision for Acceptance**
[4](#bza-provision-for-acceptance)](#bza-provision-for-acceptance)

[3.1 Purpose: [4](#purpose-1)](#purpose-1)

[3.2 Verification against requirements specification:
[4](#verification-against-requirements-specification)](#verification-against-requirements-specification)

[3.3 Validation against application context:
[4](#validation-against-application-context)](#validation-against-application-context)

[3.4 Execution of acceptance tests:
[5](#execution-of-acceptance-tests)](#execution-of-acceptance-tests)

[3.5 Defect classification:
[5](#defect-classification)](#defect-classification)

[3.6 Conclusion: [5](#conclusion)](#conclusion)

[**4.** **Submission of Acceptance Report incl. Agreed Use Cases**
[5](#submission-of-acceptance-report-incl.-agreed-use-cases)](#submission-of-acceptance-report-incl.-agreed-use-cases)

[4.1 Purpose: [5](#purpose-2)](#purpose-2)

[4.2 Verification against requirements specification:
[5](#verification-against-requirements-specification-1)](#verification-against-requirements-specification-1)

[4.3 Validation against application context:
[5](#validation-against-application-context-1)](#validation-against-application-context-1)

[4.4 Agreed use cases demonstrated:
[6](#agreed-use-cases-demonstrated)](#agreed-use-cases-demonstrated)

[4.5 Declaration: [6](#declaration)](#declaration)

## **Introduction**

This document provides the acceptance report for the *FunFlip
Educational Game*. It outlines the system under test, the provision for
acceptance, and the demonstration of agreed use cases as the basis for
formal approval.

## **SUT -- System Under Test**

### 2.1 System: {#system .unnumbered}

The *FunFlip Educational Game*, a memory card-matching application
designed for Android and iOS platforms. It is aimed at children aged
4--6 to support early learning through play.

### 2.2 Purpose {#purpose .unnumbered}

The system helps children learn vocabulary and improve memory skills by
matching card pairs, with positive audio-visual feedback and adaptive
difficulty.

### 2.3 Scope of SUT: {#scope-of-sut .unnumbered}

-   **Functional areas include:**

    -   Start screen navigation (Play, Quit)

    -   Category selection (Animals, Fruits, Vegetables)

    -   Level selection (Easy, Medium, Hard grids)

    -   Card flipping and matching logic

    -   Replay, menu navigation, quit

    -   Audio control (mute/unmute)

```{=html}
<!-- -->
```
-   **Non-functional areas include:**

    -   Performance (≤0.5 seconds response time)

    -   Usability (simple, colorful interface for children)

    -   Accessibility (voice feedback, large buttons, high contrast
        > visuals)

    -   Offline operation (runs without internet connection)

### 2.4 Technology / Architecture: {#technology-architecture .unnumbered}

-   Developed using Godot Engine 4.x

-   5-layer architecture with strict layering (UI, SceneLoader, Game
    > Logic, Data, Services)

-   Uses categories.json for card data

-   Reuses components like Card.tscn, AudioControl.gd, SceneLoader
    > (Main.gd)

### 2.5 Verification focus : {#verification-focus .unnumbered}

The system under test is the complete game, verified as a whole in
realistic usage conditions (on target devices) to ensure that it meets
both functional requirements (what the system does) and non-functional
requirements (how the system behaves).

# **BZA -- Provision for Acceptance**

### 3.1 Purpose: {#purpose-1 .unnumbered}

To document the systematic process followed for the acceptance of the
*FunFlip Educational Game* based on verification against requirements
and validation in its intended application context.

### 3.2 Verification against requirements specification: {#verification-against-requirements-specification .unnumbered}

-   All functional requirements (e.g., navigation, gameplay logic,
    > feedback) were verified against the documented specifications.

-   All non-functional requirements (e.g., performance ≤0.5s response,
    > usability, accessibility) were verified using the defined
    > measurement criteria.

-   Both positive and negative test cases were executed systematically
    > according to the test specification.

-   Results were recorded in the test protocol; no critical defects
    > (Class 1-3) remained open at the time of acceptance.

### 3.3 Validation against application context: {#validation-against-application-context .unnumbered}

-   The system was validated in realistic conditions (on Android/iOS
    > devices, offline) to ensure suitability for its intended use
    > (children aged 4--6 years).

-   The system demonstrated usability, accessibility, and responsiveness
    > appropriate for the target audience.

-   The end-to-end user journey (from start screen to gameplay to
    > completion) was validated through acceptance tests.

### 3.4 Execution of acceptance tests: {#execution-of-acceptance-tests .unnumbered}

-   System-level tests verified the integrated behavior of all
    > components.

-   The full gameplay cycle (start, category selection, level selection,
    > gameplay, replay/exit) was tested successfully.

-   Test cases covered all agreed use cases and scenarios.

### 3.5 Defect classification: {#defect-classification .unnumbered}

-   No critical defects (Class 1--3) found.

-   Minor cosmetic issues (Class 4--5) were documented but accepted as
    > non-blocking for delivery.

### 3.6 Conclusion: {#conclusion .unnumbered}

> The FunFlip Educational Game fulfills the agreed acceptance criteria.
> The system is ready for formal acceptance and handover.

# **Submission of Acceptance Report incl. Agreed Use Cases**

### 4.1 Purpose: {#purpose-2 .unnumbered}

The acceptance report provides evidence that the *FunFlip Educational
Game* meets the specified requirements and is fit for its intended use.
It serves as the formal basis for acceptance.

### 4.2 Verification against requirements specification: {#verification-against-requirements-specification-1 .unnumbered}

-   All functional and non-functional requirements were verified
    > according to the test documentation.

-   Positive and negative test cases were executed systematically.

-   No critical defects (Class 1-3) were found; minor cosmetic defects
    > (Class 4-5) were accepted.

### 4.3 Validation against application context: {#validation-against-application-context-1 .unnumbered}

-   The system was tested on target platforms (Android/iOS) in realistic
    > conditions.

-   The game was demonstrated to function as intended for the target
    > group (children aged 4--6).

-   The system was shown to be usable, accessible, and performant.

### 4.4 Agreed use cases demonstrated: {#agreed-use-cases-demonstrated .unnumbered}

-   Start Screen Navigation: Launches the app, displays the start
    > screen, allows starting or quitting the game.

-   Learning Category Selection: Enables selection of a learning
    > category (Animals, Fruits, Vegetables).

-   Level Selection: Allows selection of Easy, Medium, or Hard level
    > within a category.

-   Card Matching Gameplay: Allows flipping cards, finding pairs, and
    > receiving audio-visual feedback.

-   Level Replay / Return to Menu: After completing a level, the player
    > can replay, move to the next level, or return to the main menu.

### 4.5 Declaration: {#declaration .unnumbered}

-   All agreed use cases were successfully demonstrated. The system
    meets the acceptance criteria and is ready for formal acceptance and
    handover to stakeholders.
