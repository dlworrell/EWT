# Engineering Workbench Toolkit (EWT)

EWT is the shared engineer-facing workbench for Catalyst projects. It provides workspace management, project modeling, toolchain orchestration, debugging, packaging, and user interfaces without owning governance, engineering standards, or compliance authority.

## Authority Chain

```text
Catylist -> AES -> AEMS -> governed repositories
```

EWT is a governed repository in that chain:

- **Catylist** defines ecosystem governance and repository authority.
- **AES** defines normative engineering requirements.
- **AEMS** evaluates and enforces those requirements.
- **EWT** provides the engineer's operational toolbox.
- **Atarix, EVO, JAG, EDT, and future projects** use EWT to build, inspect, debug, package, and operate their systems.

## Scope

EWT is organized around four major subsystems:

1. **Core**
   - workspace management
   - project model
   - package management
   - configuration
2. **Toolchain**
   - assembler integration
   - C compiler integration
   - linker integration
   - image builders
3. **Debug**
   - simulator control
   - hardware debug
   - register inspection
   - tracing
   - profiling
4. **UX**
   - CLI
   - VS Code and LSP integration
   - terminal UI
   - scripting APIs

## Boundaries

EWT does not define engineering policy. It consumes AES requirements and produces artifacts and evidence that AEMS can evaluate. EDT remains the semantic document-processing platform; EWT may invoke EDT for document build or publication workflows but does not duplicate it.

## Current Phase

Architecture and bootstrap. Significant implementation should follow approved specifications and ADRs.
