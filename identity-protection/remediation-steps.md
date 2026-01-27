## Objective
Document the steps taken to respond to a suspected compromised user
using Microsoft Entra ID controls.

## Environment
Microsoft Entra ID (Free / Test tenant)

## Detection
- Reviewed sign-in logs for unusual activity
- Checked sign-in location, IP address, and authentication method
- Identified sign-in patterns that deviated from normal behavior

## Containment
- Enforced Conditional Access policy
- Required multi-factor authentication for access
- Blocked access if policy conditions were not met

## Remediation Actions
- Reset user password
- Revoked active sign-in sessions
- Blocked legacy authentication protocols

## Recovery
- Verified successful sign-in using MFA
- Confirmed access was restored only after policy compliance
- Ensured no further suspicious sign-ins occurred

## Outcome
- Unauthorized access attempts prevented
- Account secured using modern authentication
- Identity-based protections enforced

## Interview Talking Points
- Difference between containment and remediation
- Why session revocation is important
- How MFA limits the impact of credential compromise
