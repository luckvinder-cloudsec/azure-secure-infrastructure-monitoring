# Azure Project Architecture

## Overview

This project implements a secure Azure infrastructure with centralized logging and security monitoring.

## Architecture Components

1. Azure Resource Group
2. Azure Virtual Network (VNet)
3. Workload Subnet
4. Network Security Group (NSG)
5. Linux Virtual Machine
6. Azure Monitor Agent
7. Data Collection Rule (DCR)
8. Log Analytics Workspace
9. KQL-based security investigations
10. Azure Monitor Alerts

## Data Flow

Linux VM → Azure Monitor Agent → Data Collection Rule → Log Analytics Workspace → KQL Queries → Alerting

## Network Plan

- VNet address space: `10.10.0.0/16`
- Subnet: `snet-workload`
- Subnet address range: `10.10.1.0/24`
- SSH access: restricted to an authorized source IP

## Implementation Status

Architecture planned. Resources and log ingestion will be marked as completed only after successful testing.
