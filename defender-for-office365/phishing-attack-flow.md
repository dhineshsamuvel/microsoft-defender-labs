## Objective
Understand how phishing attacks occur and how Microsoft Defender for Office 365
detects and prevents them.

## Environment
Microsoft Defender for Office 365 (Free / Test tenant)

## Phishing Attack Flow
- Attacker sends a phishing email containing a malicious link or attachment
- Email reaches the user mailbox
- Safe Links rewrites URLs at delivery time
- Safe Attachments scans files in a sandbox environment

## User Interaction
- User opens the email
- User clicks the rewritten Safe Link or opens an attachment
- Microsoft evaluates the link or file at the time of interaction

## Detection and Protection
- URL reputation and detonation checks are performed
- Malicious links are blocked and a warning page is shown
- Malicious attachments are quarantined or blocked

## Why Safe Links Rewrites URLs
- Enables time-of-click protection
- Protects against delayed or newly weaponized links
- Provides visibility into user interaction

## Response Behavior
- Access to malicious content is prevented
- Email may be quarantined automatically
- Activity is recorded in the Defender portal

## Outcome
- Phishing attempts are detected before user compromise
- Risk of credential theft is reduced
- Email security controls enforce protection without user action

## Interview Talking Points
- Why email is a common attack vector
- Purpose of URL rewriting
- Difference between delivery-time and click-time protection
