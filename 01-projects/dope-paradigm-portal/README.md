# Dope Paradigm Portal

## What It Is

**Dope Paradigm Portal** is the internal macOS operator portal used to manage catalog records, media workflows, imports, and admin-side visibility across the music system.

## Role in the Ecosystem

Dope Paradigm Portal is the control surface behind much of the public-facing music experience. It helps shape the catalog and operator workflows that eventually feed the fan-facing app.

## Audience

- internal operator use
- admin use
- catalog management
- publishing workflow support

## Platform

- macOS
- Web (Coming soon)

## Current Focus

Current work has focused on:
- Apple Music import workflows
- cleaner operator review flows
- metadata visibility
- import reruns without duplication
- dashboard metrics and admin controls
- safer destructive tooling separation

## Recent Milestones

- Apple Music import became a real working workflow
- full release metadata handling improved across imports
- import categories were normalized into Albums, EPs, Singles, and Tracks
- dashboard metrics were split into better long-term categories
- realtime dashboard behavior became an operator setting instead of an assumption

## Framework / Feature Notes

At a high level, Dope Paradigm Portal currently uses:
- SwiftUI
- Firebase Auth
- Firestore
- Apple Music / MusicKit

## Status

Active internal system.

Dope Paradigm Portal is the operational bridge between the private system and the public fan experience.
