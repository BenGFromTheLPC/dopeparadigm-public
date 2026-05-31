# 2026-05-30 — Dope Paradigm HQ Guest Browsing and Dope Paradigm Portal Clean Release Labeling

This round of work focused on smoothing out guest-mode behavior in Dope Paradigm HQ and making clean-release metadata easier to read inside Dope Paradigm Portal.

## Project

- Dope Paradigm HQ
- Dope Paradigm Portal

## What Changed

- guest album browsing in Dope Paradigm HQ was tightened so album taps open the album experience instead of dropping into the wrong gate state
- guest playback prompts were made more consistent across album play, album shuffle, and recently updated track surfaces
- the welcome-to-guest transition in Dope Paradigm HQ now fades into the live catalog instead of snapping abruptly
- clean albums and clean tracks now surface a dedicated badge in Dope Paradigm Portal across all albums, all tracks, and album detail views
- the clean-release badge styling in Dope Paradigm Portal was shifted to a neutral gray treatment so it does not visually compete with the live status

## Why It Matters

Small consistency issues are the kind of thing that make an app feel rough even when the larger architecture is sound. This pass helped the guest experience feel more intentional in Dope Paradigm HQ while giving the operator-facing catalog in Dope Paradigm Portal clearer metadata cues for clean releases.

## High-Level Stack Notes

This work touched:
- SwiftUI
- Firebase / Firestore-backed catalog data
- Apple Music-connected playback flows
- shared release metadata surfaced across fan-facing and operator-facing apps

## Public-Safe Summary

The system is getting better at two important product layers at the same time: guest users can move through the music experience more smoothly, and operator tools are showing cleaner release-state details without adding visual clutter.
