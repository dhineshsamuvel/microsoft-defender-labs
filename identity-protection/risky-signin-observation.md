## Objective
Understand how risky sign-ins and risky users are evaluated
in Microsoft Entra ID.

## Environment
Microsoft Entra ID (Free / Test tenant)

## Observation
Risky sign-in and risky user data was not visible in this environment.

## Reason
Risk-based identity protection features require Microsoft Entra ID P2 licensing.
This tenant is using a free or limited trial license.

## Expected Risk Signals (Licensed Environment)
Risk signals may be generated based on:
- Sign-in from unfamiliar locations
- Impossible travel scenarios
- Anonymous or VPN-based IP addresses
- Suspicious sign-in behavior patterns

## Risk Types
- Sign-in risk: Indicates a suspicious authentication attempt
- User risk: Indicates a higher likelihood that the account is compromised

## Policy Behavior (If Risk Detected)
- Medium sign-in risk: Require multi-factor authentication
- High user risk: Block access until risk is remediated

## Validation
- Reviewed standard sign-in logs
- Verified Conditional Access policy evaluation
- Confirmed MFA enforcement during sign-in

## Interview Talking Points
- Difference between sign-in risk and user risk
- Why risky sign-ins may not appear in free tenants
- How Conditional Access responds to identity risk
