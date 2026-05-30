# PicPull

## What It Is

**PicPull** is an anonymized internal macOS utility for importing photos and videos from trusted iPads into a structured local folder on a Mac. It is designed to make media transfer feel deliberate and operational rather than ad hoc, with clear device status, destination control, progress visibility, and post-copy verification.

## Problem It Helped Solve

This app was built to reduce friction around pulling media off managed tablets during real production workflows. The main challenge was creating a repeatable import process that gave the operator confidence about where files were going, what was being copied, and whether the transfer actually completed correctly.

## Audience

- internal creative and content operations staff
- operators handling device offload and media intake
- teams organizing photo and video assets for downstream editing or archive workflows

## Platform

- macOS

## Use Case

PicPull is meant for the moment when a trusted iPad is plugged into a Mac and its local media needs to be copied into a known folder structure with verification. It supports practical intake scenarios where the operator wants a fast answer to: did the device connect, which media is being imported, where is it going, and did every file land successfully.

## Structure and Workflow Design

At a high level, the app is organized around one focused desktop workflow:

- device detection surfaces connected iPads and makes readiness states explicit
- destination selection lets the operator choose the export folder and set a device-specific import folder name
- media filtering supports photos-only, videos-only, or combined imports
- folder-layout options support either a flat export or separated photo/video subfolders
- copy progress, elapsed time, and verification feedback make the transfer state easy to monitor
- optional HEIC-to-JPEG conversion supports workflows that need more common image outputs while preserving the original files in an archive folder

## Framework / Feature Notes

At a high level, this project currently uses:

- SwiftUI
- ImageCaptureCore
- ImageIO
- AppKit where macOS-native file picking is needed
- local file-system workflows for copy, verification, and export organization

## Why It Mattered

What made this app useful was not just copying media, but turning media intake into a more trustworthy workflow. Instead of treating import as a black box, PicPull gives the operator a controlled desktop flow with explicit status, predictable folder structure, and a verification step that helps reduce uncertainty after the transfer finishes.

## Public-Safe Summary

PicPull is a private internal macOS media-ingest tool for importing and verifying photo and video assets from connected iPads. It shows how a focused Apple-platform utility can turn a routine operational task into a more reliable desktop workflow without exposing private process details or internal implementation logic.

## Status

Active internal macOS utility focused on device media intake, verification, and workflow refinement.
