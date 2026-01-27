## Objective
Implement identity-based access controls using Microsoft Entra ID
to reduce the risk of account compromise.

## Environment
Microsoft Entra ID (Free / Test tenant)

## Configuration Performed
- Created Conditional Access policy for sign-in risk
- Required MFA for medium-risk sign-ins
- Blocked access for high user risk
- Disabled legacy authentication protocols

## Security Rationale
Identity-based attacks often succeed after credential theft.
Conditional Access evaluates sign-in context such as risk level,
authentication method, and user behavior before granting access.

Blocking legacy authentication prevents bypass of modern security
controls such as MFA.

## Outcome
- MFA enforced for risky sign-ins
- High-risk users blocked from accessing resources
- Legacy authentication attempts denied

## Validation
- Conditional Access policy evaluated during sign-in
- MFA challenge triggered when conditions were met
- Sign-in logs reflected policy enforcement

## Interview Talking Points
- Difference between user risk and sign-in risk
- Why Conditional Access is preferred over per-user MFA
- How MFA reduces the impact of credential compromise
