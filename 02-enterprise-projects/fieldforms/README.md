# FieldForms

## What It Is

**FieldForms** is an anonymized internal iPadOS workflow app for structured field form submission. It is designed to turn recurring workforce paperwork into a guided digital flow with draft saving, signature capture, generated output files, and controlled submission tracking.

## Problem It Helped Solve

The app was built to replace manual and inconsistent field form handling. The core challenge was creating a repeatable way for teams to complete operational forms accurately, collect required signatures, preserve draft progress, and submit records without relying on paper-first workflows.

## Audience

- field personnel completing recurring forms
- supervisors and approvers involved in signoff workflows
- internal operations staff reviewing submission history

## Platform

- iPadOS

## Structure and Workflow Design

At a high level, the app is organized around a practical end-to-end form workflow:

- apprentice and form-type selection routes users into the correct form path
- form screens support required validation, comments, and digital signature capture
- draft persistence and restore flows reduce data loss during interrupted sessions
- generated PDF and spreadsheet outputs preserve a structured local record
- submission requests trigger automation flows that archive records and notify internal teams
- submission-history views support operational follow-through and traceability

## Framework / Feature Notes

At a high level, this project currently uses:

- SwiftUI
- SwiftData
- URLSession
- Apple's Network framework (connectivity monitoring)
- PDF generation on Apple platforms
- local file persistence for generated artifacts
- Microsoft Power Automate for downstream workflow orchestration
- SharePoint as an internal document destination for submitted artifacts
- Microsoft Teams notifications for internal visibility after successful submission

## Submission and Internal Delivery Flow

At a high level, submission behavior is designed around operational reliability:

- FieldForms generates a PDF and spreadsheet-style export during submission
- the app sends the payload into Power Automate endpoints
- Power Automate stores the submitted files in SharePoint
- Power Automate posts a Teams message with a link to the SharePoint files so internal stakeholders can open the submitted record quickly

## Network Awareness and Fallback Behavior

FieldForms includes network-detection safeguards to reduce failed submissions:

- submissions are disabled when the iPad is offline
- the app warns users when connectivity is weak (Wi-Fi or cellular), indicating submissions may fail or return an error
- if a network error occurs, local copies of generated files remain available on the iPad
- those local files can be moved manually when needed (for example via AirDrop, external storage, or email)

## Distribution Approach

FieldForms was packaged as an internal **IPA** build, then deployed through **Microsoft Intune** for managed internal distribution. This allowed the app to be installed on enrolled organization-managed iPads without a public App Store release, while keeping rollout and access controlled through enterprise device management policy.

## Why It Mattered

This project improved operational consistency by giving teams one standardized iPad workflow for form completion, signature capture, and submission tracking. It reduced manual handoff friction, improved record quality, and made internal distribution manageable through existing device-management channels.

## Public-Safe Summary

FieldForms is a private internal iPadOS operations app for structured form workflows. It demonstrates how a focused Apple-platform tool can combine guided input, local artifact generation, managed enterprise distribution, and connected Microsoft workflow automation without exposing sensitive internal process details or private implementation logic.

## Status

Active internal tool with ongoing iteration around workflow reliability and form operations.
