# Secure C/C++ Profile

Status: Adopted
Repository: dlworrell/EWT
Inherited Standard: AES-SEC-001

## Purpose

EWT is planned as a standalone, C-based engineering workbench. Although the
current repository is in architecture and bootstrap, it adopts the secure native
baseline now so future implementation begins inside the governed boundary.

## Required Local Behavior

Future C or C++ code must:

- avoid AES-SEC-001 banned interfaces;
- carry explicit lengths for external buffers and toolchain inputs;
- validate file, package, protocol, and debugger data before use;
- check allocation and size arithmetic for overflow;
- isolate platform-specific unsafe operations behind reviewed interfaces;
- compile cleanly under the repository warning and Clang-Tidy profile;
- run sanitizer tests where the target permits;
- fuzz parsers and externally controlled inputs when applicable; and
- document every approved exception in the waiver log.

## Authority Boundary

AES defines the normative rules. AEMS evaluates compliance. This file records
EWT's local adoption and does not create independent policy.

## Ratchet Rule

The repository begins with a zero-violation baseline. New violations block merge
unless an explicit, reviewed waiver is recorded.
