# Satori Video Library Establishes a Cleaner Shared-System Boundary

Satori and Satori Portal now share a dedicated Tabularium-owned contract layer
for the emerging personal video library. The change keeps the operator tools
aligned while preserving a clean boundary around the internal engine used by
other apps in the Dope Paradigm ecosystem.

## Project

- Satori
- Satori Portal
- Tabularium

## What Changed

- Built the first phase of a folder-organized video library with a vertical
  mobile feed, quick sharing, desktop management, and a batch upload workflow.
- Added a dedicated shared model layer for video-library folders, tags, assets,
  edit details, and feed ordering.
- Connected the iOS and macOS operator apps to the same pinned contract version.
- Kept the broader internal app engine separate from the video-library workflow.
- Verified the shared package, upload-queue behavior, feed behavior, and both
  application builds.

## Why It Matters

The separation gives Satori and Satori Portal one consistent vocabulary without
coupling their video workflow to unrelated app features. Tabularium remains
the cloud memory and state layer, while each app keeps a focused responsibility.

## High-Level Stack Notes

- Swift and SwiftUI
- Swift Package Manager
- Firebase and Firestore
- Tabularium shared cloud state

## Public-Safe Summary

The Satori operator tools now share a dedicated Tabularium contract layer for
video-library work, improving consistency while keeping the wider Dope Paradigm
app architecture intentionally separated.
