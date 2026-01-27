## Objective
Understand how Microsoft Defender correlates multiple security signals
into a single incident for effective investigation.

## Environment
Microsoft Defender (Free / Test tenant)

## Observation
No real security incidents were generated during the lab period.

## Reason
- Free trial tenant with limited alert generation
- No active real-world malicious activity
- Simulated attacks may not trigger full incident creation

## Correlation Logic
Microsoft Defender groups related alerts based on:
- Common user accounts
- Email activity
- URL or attachment interaction
- Time-based relationships between events

## Example Correlated Flow
- Phishing email delivered to mailbox
- User clicks a suspicious link
- URL reputation changes after delivery
- Sign-in activity reviewed for anomalies
- Related detections grouped as a single incident

## Automated Investigation
Defender automatically analyzes:
- Email content and headers
- URLs and attachments
- User activity related to the email

## Outcome
- Alerts are grouped into one incident
- Timeline provides clear event sequence
- Investigation status indicates threat verdict

## Validation
- Incidents and alerts dashboard reviewed
- Correlation workflow studied using phishing simulation data
- Incident timeline and entity views explored

## Interview Talking Points
- Difference between alerts and incidents
- Benefits of incident correlation
- How timelines help understand attack progression
