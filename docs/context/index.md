# Contexts

Contexts are defined as the FreeBSD operating system context where a helper script or configuration should reside, being either in the root FreeBSD operating system, within jails, or both. Each helper script and configuration has a context defined in its header where it is best suited to be used. Those contexts are defined below.

## Defined Contexts

### NOJAIL

This script or configuration should reside *only* within the root FreeBSD operating system (not within jails).

### JAILONLY

This script or configuration should reside *only* within FreeBSD jails (not within the root operating system).

### ANY

This script or configuration should reside within either the root FreeBSD operating system, or its jails.

## Example Definition

The context header within a helper script or configuration may look like this:

```
# Version: 1.0.0
# Context: ANY                 Can be used in host OS or jails
# (Read more: https://hackthiscode.github.io/FreeBSD-Helpers/context/ )
```
