# GearGate / GearGateTV

## What It Is

**GearGate** is an anonymized internal device operations system built around iPad/radio checkout, return tracking, accessory accountability, live queue visibility, and signed workflow documentation. It includes an iPadOS app for hands-on workflow execution and an Apple TV companion app that turns the same workflow into a shared room-level dashboard.

## Problem It Helped Solve

This system was built to replace fragmented tracking around shared mobile equipment. The challenge was not only knowing who had a device, but making checkout, return, condition tracking, deduction paperwork, and live queue communication feel fast, consistent, and trustworthy in a real operational environment. It also needed a stronger paper trail around damaged devices, returned equipment, and signed accountability records.

## Audience

- internal technology staff
- field supervisors and coordinators
- workers checking devices in and out
- teams monitoring live pickup and waiting queues

## Platform

- iPadOS
- tvOS

## Structure and Workflow Design

At a high level, the system is split into two connected surfaces:

- **GearGate for iPadOS** handles device checkout and return workflows, equipment record selection, accessory tracking, return status capture, signature collection, PDF generation, and outbound HTTP requests into connected automation.
- **GearGateTV for Apple TV** acts as a live operational dashboard showing pickup queues, waiting lists, and task-style visibility in a format designed for a larger shared screen.
- The system is built around an Excel spreadsheet stored in SharePoint as the source of truth for device records.
- Power Automate is used to query current available devices during checkout flows and current checked-out devices during return flows so users are choosing from live records instead of stale lists.
- Checkout forms, return forms, and deduction-related documents are generated from the workflow, saved into SharePoint, and emailed to relevant stakeholders for follow-up and recordkeeping.
- Together, the workflow moves device events from mobile input to generated forms, automation, and signed recordkeeping without depending on a paper-first handoff.

## Framework / Feature Notes

At a high level, this project currently leans on:

- SwiftUI
- URLSession
- SharePoint-backed operational records
- Excel-based source-of-truth workflow design
- Power Automate HTTP flows
- PDF generation on Apple platforms
- tvOS dashboard patterns for shared-screen visibility
- HTTP-based workflow integration
- JSON-driven automation endpoints
- signature capture and device form workflows

## Distribution Approach

The iPadOS app is distributed privately through **App Store Connect** using **App Distribution Methods** rather than as a public App Store release. That keeps the app available for controlled internal use while preserving a clean separation between workforce tooling and public-facing software.

## Why It Mattered

What made this project valuable was the combination of accountability, speed, and visibility. The iPad app gave the workflow a structured front door, while the Apple TV layer made it easier for people in the room to see what was ready, what was waiting, and where the queue stood without every user needing direct access to the internal app itself. Just as important, the workflow created a clearer paper trail around device damage, returned equipment, and signed forms so operational decisions were easier to track and defend over time.

## Public-Safe Summary

GearGate is a private internal Apple-platform workflow system for managing shared device operations. It shows how custom iPadOS software, a companion Apple TV dashboard, SharePoint-backed records, and Power Automate workflows can work together to improve equipment handling, queue visibility, signed accountability, and operational clarity without exposing the private business logic or internal infrastructure behind the workflow.

## Status

Active internal tool with ongoing refinement across both the iPadOS app and the Apple TV dashboard.
