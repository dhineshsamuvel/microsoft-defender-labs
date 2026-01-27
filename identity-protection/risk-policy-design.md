## Objective
Design risk-based access policies to protect user identities
using Microsoft Entra ID.

## Environment
Microsoft Entra ID (Free / Test tenant)

## Risk-Based Design Approach
Access decisions are made based on the level of risk
associated with a user or a sign-in attempt.

## Risk Types Considered
- Sign-in risk: Indicates a suspicious authentication attempt
- User risk: Indicates a higher probability that an account is compromised

## Policy Design
- Medium sign-in risk:
  - Require multi-factor authentication
- High user risk:
  - Block access until the risk is resolved
- Legacy authentication:
  - Blocked to prevent MFA bypass

## Security Rationale
Risk-based policies reduce unnecessary access restrictions
while applying stronger controls only when suspicious activity
is detected.

Blocking high-risk users prevents further misuse of
potentially compromised credentials.

## Outcome
- Normal users experience minimal friction
- Risky sign-ins are challenged with MFA
- High-risk accounts are prevented from accessing resources

## Validation
- Conditional Access policy configuration reviewed
- Policy evaluation observed in sign-in logs
- MFA enforcement confirmed during authentication

## Interview Talking Points
- Why risk-based access is better than static rules
- Difference between sign-in risk and user risk
- How Conditional Access supports Zero Trust principles
