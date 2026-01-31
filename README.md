# DeviceRegistry_Lander

# Device Registry

**Status:** Experimental  
**Scope:** Naming only  
**Governance:** None (owner-maintained, opt-in usage)

## Overview

Device Registry is an ENS-based naming convention rooted at `device.eth`.

It provides a neutral namespace for identifying devices — physical or virtual —
that execute actions on behalf of humans, organizations, or software systems.

The registry does not define behavior, permissions, or security models.
It exists solely to make device identity nameable and referenceable.

## Motivation

Most systems conflate identity across multiple layers:
- humans
- agents
- devices

This leads to over-scoped authority and coarse revocation.
When a device is compromised, entire accounts are rotated.

Explicit device identity allows systems to answer:
- which device executed this action?
- under whose authority?
- can this specific device be revoked?

## Naming Model

All device identifiers are subnames of `device.eth`.

Examples:
phone.device.eth
laptop.device.eth
robot.device.eth
sensor.device.eth
server.device.eth

Names are descriptive, not prescriptive.
Interpretation is left to consuming systems.

## Ownership & Delegation

- `device.eth` is owned by a single ENS owner
- Subnames may be issued, delegated, revoked, or expired
- The registry makes no assumptions about trust or duration

## Records & Metadata (Optional)

Subnames may include ENS records such as:
- associated public keys
- device type descriptors
- timestamps or notes

All metadata is optional and non-normative.

## Non-Goals

Device Registry explicitly avoids:
- defining standards
- enforcing policies
- replacing vendors
- acting as a protocol or platform

## Intended Use

The registry serves as:
- a reference point in documentation
- a shared vocabulary for device identity
- a neutral naming layer

Adoption is voluntary and non-exclusive.

## Versioning

This document describes v0.1 of the Device Registry concept.
Future revisions may clarify conventions while preserving compatibility.
