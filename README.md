# engineering-handbook

## On-Call

To scale our infrastructure we have a dev-ops culture including 24/7 support with rotating on-call. Conditions for this is documented in [Google Drive](https://docs.google.com/document/d/1vEP3QwE2EVNqQ6D7FjIIQAwhZe6pXnkfZQvt1vr7OAM/edit).

## Quality

Quality is everyone's responsibility! Everything you merge to master should be production ready. 

### Zero bug policy

We shall treat quality as an important part of our product and shall therefore act accordingly. In addition we shall set clear expectations on resolutions on issues and not have issues in the backlog for an extended period of time. Therefore we adhere to a “zero bug” policy. 
When we discover bugs we triage the bug as soon as possible in the team most fitted to evaluate customer impact of the issue. If customer impact is unclear it is the Product Manager’s role to decide on the severity of the issue. 
- **Critical issue:**
	Stop current work and attend the issue expeditly.
- **High impact issue:** 
	Plan the work coming week or as soon as possible without the intrution of a “drop everything”.
- **Medium impact issue:**
	Plan the work within the coming three weeks and solve the issue.
- **Low impact issue:**
	Close the issue as we will not be able to prioritize low impact issues. Repeat the process if and when the same bug appear in the future.

To help ensure we adhere to this agreement we have a dashboard showing inflow / resolution for the different platforms. In addition there is a weekly review of bugs older then 3 weeks to validate that the issues older are acted on in a timely manner. 

### Crashes

Client crashes are tracked in Firebase by Crashlytics. We treat all crashes as bugs and prioritize it according to the bugs. Our aim is to be above **99.5%** crash rate.

If the Crash rate drops below **99.0%** it is considered an incident and shall be acted on with equal urgency.
