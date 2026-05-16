# Vertical Slice Architecture

This repository contains the canonical Vertical Slice Architecture guidelines used by this workspace. The authoritative specification lives in [VSA.md](./VSA.md), which defines the solo-agent operating model, slice boundaries, shared-kernel constraints, data sovereignty rules, observability requirements, and refactoring triggers.

## Overview

Vertical Slice Architecture organizes code around business capabilities rather than technical layers. The goal is to keep each slice self-contained so that ownership, change isolation, and boundary enforcement stay explicit.

## What the specification covers

- Slice terminology and responsibility boundaries
- Mandatory slice anatomy: entry point, input model, validator, handler, and `CONTEXT.md`
- File naming rules for slices, shared kernel concepts, and tests
- Validation, error handling, and result-flow expectations
- Data ownership, cross-slice read/write boundaries, and integration events
- Structured observability and error-envelope requirements
- Refactoring triggers and hard gates for autonomous execution
- Context-scaling guidance for small, medium, and large slice counts

## Repository layout

- [VSA.md](./VSA.md): Canonical guidelines and rule set
- [Archive/](./Archive): Historical XML and Markdown exports kept for reference
- [LICENSE](./LICENSE): GNU license

## How to use this repo

1. Start with [VSA.md](./VSA.md) when you need the current rules.
2. Use [Archive/](./Archive) only for historical comparison or version recovery.
3. Treat [VSA.md](./VSA.md) as the source of truth when reviewing or generating slice code.

## License

This repository is released under the GNU License. See [LICENSE](./LICENSE) for details.
