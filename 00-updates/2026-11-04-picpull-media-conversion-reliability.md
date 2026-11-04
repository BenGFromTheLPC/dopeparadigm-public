# 2026-11-04 — PicPull: Media Conversion Reliability

PicPull's media-import workflow was refined to keep compatibility conversion responsive and aligned with current macOS frameworks while preserving the operator's original files.

## Project

- PicPull
- Platform: macOS

## What Changed

- Moved image compatibility conversion away from UI-critical work so longer imports remain responsive.
- Modernized video conversion and metadata handling for current macOS media APIs.
- Preserved HEIC-to-JPEG and MOV-to-MP4 compatibility workflows with original-file archive folders.
- Tightened import progress ownership and cleared current source-level build warnings.

## Why It Matters

Media intake can involve thousands of files, so conversion work needs to stay dependable without making the desktop workflow feel stalled. These refinements keep PicPull focused on visible progress, preserved originals, and outputs that fit common downstream editing and archive workflows.

## High-Level Stack Notes

- SwiftUI
- ImageCaptureCore
- ImageIO
- AVFoundation

## Public-Safe Summary

PicPull's photo and video compatibility pipeline is now more responsive and current with macOS media frameworks, while continuing to preserve originals and verify the files produced during import.
