# Day 1 – Azure Policy Deep Dive

## Scenario

Prevent public exposure of Azure resources by denying Public IP creation.

## Problem

Public IP addresses increase attack surface and are often restricted in enterprise environments.

## Solution

Implemented Azure Policy with deny effect targeting:

* Microsoft.Network/publicIPAddresses

## Result

Deployment blocked with:

* RequestDisallowedByPolicy

## Reflection

* Policy enforcement happens at deployment time
* Clear error messages help debugging
* Governance must be automated and version-controlled

## Next Improvement

* Add audit policies
* Implement policy initiatives

