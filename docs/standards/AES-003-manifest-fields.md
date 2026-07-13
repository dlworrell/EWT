# AES-003 Supporting Document: Manifest Field Requirements

Status: Draft
Owner: AES
Parent: AES-003 Repository Manifest Standard

## Purpose

Define the initial field set expected in a Catalyst repository manifest.

## Core Fields

A governed repository should provide fields for:

- manifest version
- repository identifier
- repository name
- repository owner
- repository role
- lifecycle state
- Project Zero state
- applicable AES standards
- primary branch
- issue tracker

These fields provide the minimum information needed for repository discovery, lifecycle reporting, and AEMS inspection.

## Supplemental Fields

A repository may also provide fields for:

- contacts
- labels
- dashboards
- release policy
- certification history
- related repositories
- documentation roots
- generated reports
- accepted deferrals

Supplemental fields should not contradict core repository identity, lifecycle, ownership, or standards information.
