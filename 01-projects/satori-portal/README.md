# Satori Portal

## What It Is

**Satori Portal** is the macOS operator interface for managing the music-catalog side of the Dope Paradigm ecosystem. It is where releases, cover art, promo media, links, and track-level details can be organized from a larger desktop surface.

## Role in the Ecosystem

If Satori is the mobile control layer, Satori Portal is the desktop management layer. It gives the ecosystem a place to shape catalog data, upload public-facing media assets, and keep release information organized before that state appears in connected experiences.

Satori Portal works with **Tabularium**, the shared cloud memory and state system for Dope Paradigm. Tabularium lets Portal act as a control surface while keeping the catalog state available to Satori and future internal tools.

## Audience

- internal admin/operator workflows
- music catalog management
- promo media organization
- release and track metadata review
- future ecosystem control workflows

## Platform

- macOS
- Web direction planned for the future

## Current Direction

Satori Portal is currently focused on:

- music release creation and editing
- album and single metadata management
- front and back cover handling
- Apple Music promo image and video organization
- release link management
- track lists, track numbering, and track-level metadata
- track-level promo content uploads
- local error visibility for debugging upload flows
- Tabularium-backed cloud memory/state for the catalog

## Recent Notable Work

- Expanded the release detail workflow for albums and singles.
- Added front and back cover handling with preview and delete states.
- Added release links with edit, delete, and copy behavior.
- Added album tracks with ordering, numbering, editing, and deletion.
- Added track-level promo image and video management.
- Connected Portal-managed catalog data to Satori on iOS through the shared Tabularium-backed state layer.

## Why It Matters

Satori Portal makes the internal catalog workflow more intentional. Instead of managing release details, links, promo assets, and track data across disconnected places, Portal gives the ecosystem a desktop control surface that can feed mobile review, future automation, and public-facing experiences.

## Public-Safe Summary

Satori Portal is a private macOS admin tool connected to Tabularium, the Dope Paradigm cloud memory system. It manages music release metadata, promo assets, links, and track-level catalog information without exposing private implementation details or internal system wiring.

## Status

Active internal macOS tool, currently centered on catalog management and Tabularium-backed music release workflows.
