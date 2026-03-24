# Azure Enterprise Security Platform

## Overview

This repository contains my hands-on learning journey for Azure security, governance, and platform engineering.

---

# Day 1 – Azure Policy Fundamentals

## Objective

Understand and implement Azure Policy to enforce security controls.

## What I implemented

* Created a custom Azure Policy:

  * Deny creation of Public IP addresses
* Assigned the policy at subscription level

## Testing

* Attempted to create a Public IP resource
* Deployment failed with policy violation:

  * Error: RequestDisallowedByPolicy

## Key Learning

* Azure Policy enforces rules at deployment time
* Deny effect prevents insecure configurations
* Policy evaluation shows exactly why a resource is blocked

## Real-world relevance

* Preventing public IP exposure is a common enterprise security requirement
* This type of policy is used in secure landing zones

## Next Steps

* Implement audit policies
* Explore Azure Security Benchmark

