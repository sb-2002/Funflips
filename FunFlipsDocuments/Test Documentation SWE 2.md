---
title: Test Documentation
---

Project: FunFlip Game

Authors:

Ashish Ghaskata\
Krishna Raj Bhandari

Suraj Bhatta

Mohammad Adnan Khan

**Documentname:** AB-Funflip Game-Test Doc

**Creation date:** 20.06.2025

Table of Contents

[1. Introduction [2](#introduction)](#introduction)

[1.1 Purpose [2](#purpose)](#purpose)

[1.2 Scope [2](#scope)](#scope)

[2. Test Specification [2](#test-specification)](#test-specification)

[Test Cases [2](#test-cases)](#test-cases)

[3. Test Protocol [5](#test-protocol)](#test-protocol)

[Test Results Summary [5](#test-results-summary)](#test-results-summary)

[Defect Log [6](#defect-log)](#defect-log)

[Conclusion [6](#_Toc201627892)](#_Toc201627892)

[References [6](#references)](#references)

# 

# 1. Introduction

## 1.1 Purpose

This document specifies the test plan and protocol for the FunFlip
educational game, ensuring all functional and non-functional
requirements are validated.

## 1.2 Scope

Covers all game functionalities including start screen, navigation,
gameplay logic, UI feedback, and performance.

# 2. Test Specification

Each test case includes:

-   Name

-   Tested Requirement

-   Precondition

-   Postcondition

-   Test Steps

-   Expected Result

-   Test Infrastructure

## Test Cases

**TC01: Start Screen Display**

-   **Tested Requirement**: Start screen loads within 0.5s

-   Precondition: App installed and launched

-   Postcondition: Start screen visible

-   Test Steps: Launch app

-   Expected Result: Start screen appears within 0.5s

-   Test Infrastructure: Mobile device, stopwatch

**TC02: Play Button Navigation**

-   Tested Requirement: Play button leads to category selection

-   Precondition: On start screen

-   Postcondition: Category selection visible

-   Test Steps: Tap Play button

-   Expected Result: Category selection appears

-   Test Infrastructure: Mobile device

**TC03: Quit Button Functionality**

-   Tested Requirement: App exits on Quit button

-   Precondition: On start screen

-   Postcondition: App closes

-   Test Steps: Tap Quit button

-   Expected Result: App exits

-   Test Infrastructure: Mobile device

**TC04: Category Selection**

-   Tested Requirement: Category selection works

-   Precondition: On category selection screen

-   Postcondition: Level selection screen shown

-   Test Steps: Tap category

-   Expected Result: Level selection loads

-   Test Infrastructure: Mobile device

**TC05: Level Selection**

-   Tested Requirement: Level selection loads correct grid

-   Precondition: On level selection screen

-   Postcondition: Game board loads

-   Test Steps: Tap level

-   Expected Result: Game board displayed

-   Test Infrastructure: Mobile device

**TC06: Card Match Success**

-   Tested Requirement: Matching cards stay revealed

-   Precondition: Game board loaded

-   Postcondition: Matched cards remain visible

-   Test Steps: Flip two matching cards

-   Expected Result: Cards stay revealed, sound plays

-   Test Infrastructure: Mobile device, Godot debugger

**TC07: Card Match Failure**

-   Tested Requirement: Mismatched cards flip back

-   Precondition: Game board loaded

-   Postcondition: Cards flip back

-   Test Steps: Flip two non-matching cards

-   Expected Result: Cards flip back after delay

-   Test Infrastructure: Mobile device, Godot debugger

**TC08: Audio Toggle**

-   Tested Requirement: Audio can be muted/unmuted

-   Precondition: Game running

-   Postcondition: Audio state changes

-   Test Steps: Mute audio in options

-   Expected Result: Audio is muted

-   Test Infrastructure: Mobile device

**TC09: Back Button Handling**

-   Tested Requirement: Back button navigates or debounces

-   Precondition: On any screen

-   Postcondition: Previous screen or no effect on spam

-   Test Steps: Tap back repeatedly

-   Expected Result: One back action processed

-   Test Infrastructure: Mobile device

**TC10: Response Time Validation**

-   Tested Requirement: Action response within 0.5s

-   Precondition: Game board loaded

-   Postcondition: Action completed

-   Test Steps: Flip card

-   Expected Result: Card flips in ≤0.5s

-   Test Infrastructure: Stopwatch, mobile device

# 3. Test Protocol

## Test Results Summary

  -----------------------------------------------------------------------
  **Test Case**           **Result**              **Notes**
  ----------------------- ----------------------- -----------------------
  TC01                    Pass                    Start screen loaded
                                                  fast

  TC02                    Pass                    Play button worked

  TC03                    Pass                    Quit button closed app

  TC04                    Pass                    Category selection
                                                  worked

  TC05                    Pass                    Level loaded correctly

  TC06                    Pass                    Match logic correct

  TC07                    Pass                    Mismatch handled

  TC08                    Pass                    Audio toggle functional

  TC09                    Pass                    Back button debounced

  TC10                    Pass                    Flip response within
                                                  time
  -----------------------------------------------------------------------

## Defect Log:

  -----------------------------------------------------------------------
  **Test Case**           **Defect Class**        **Description**
  ----------------------- ----------------------- -----------------------
  TC07                    5 (Cosmetic)            Slight delay in card
                                                  flip-back beyond ideal
                                                  timing

  TC04                    4 (Small deviation)     Minor button alignment
                                                  issue on category
                                                  selection screen
  -----------------------------------------------------------------------

[]{#_Toc201627892 .anchor}Conclusion:\
All mandatory functional and non-functional requirements were fulfilled.
No critical defects (Class 1--3) were found. Minor cosmetic issues were
documented and accepted as non-blocking for delivery.

## 4. References

-   Requirements Documentation

-   Architectural Documentation

-   SWE_SoSe2025_DELIVERABLES.pdf

-   tasks3_document-check-list.pdf

-   swe_05_test.pdf
