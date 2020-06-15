# Introduction

The Fishbrain engineering handbook is the central repository for how we run the engineering teams. As part of our value of being transparent the handbook we aim to publish these pages to make access easier for everyone.

We welcome feedback. Please make a [pull request](https://github.com/fishbrain/engineering-handbook/pulls) to suggest improvements or add clarifications. Please use [issues](https://github.com/fishbrain/engineering-handbook/issues) to ask questions.

## Sections

- [Quality](./Quality/README.md)
- [Fishway](./Fishway/README.md)


## Keeping yourself informed

* Email lists
	- Product team mailing list
	- Platform team mailing list
	- Engineering mailing list

Become members as part of the onboarding process. If this is not the case for you, reach out to your manager

* Slack
	- #information
	- #everybody
	- #development
	- #bugs
	- #alerts

If you frequently check these channels, you can consider yourself informed.

## Other Related Pages

* [Fishbrain knowledge](https://docs.fishbrain.com/)
* [Fishbrain documentation](https://github.com/fishbrain/docs)

## On-Call

To scale our infrastructure we have a dev-ops culture including 24/7 support with rotating on-call. Conditions for this is documented in [Google Drive](https://docs.google.com/document/d/1vEP3QwE2EVNqQ6D7FjIIQAwhZe6pXnkfZQvt1vr7OAM/edit).

## Incident management

When we have a incident it is important that we have a uniformed way of acting to the incidents. This will reduce the load on the on-call person and ensure we do the right things at the time of the incident. If there is a incident it will be in the #alert channel in slack and all dialogs about ongoing incidents shall be held there. If there is a outage or another need to get the attention of the on-call person there is a slack command "/pd trigger" that will fire an manual alert. Note that if the alert needs to reach the CTO it is done through PagerDuty and can be done by anyone on-call.
For all incidents that is impacting our users it is important to share the information witin Fishbrain in a transperent way so we can be proactive and honest wit our users. Bigger incidents shall be shared in #everybody and minor ones in #support.

### Security incident
We have a documented security incident response plan that is used for any security and data incidents and details the work needed and the authorities that needs to be informed in [Google Drive] (https://docs.google.com/document/d/1H5CvNvs6YesRPdjf2KcP4Vz2Z7nmpNOnJm_XB2dBWSU/edit).

### Backend failures
We have a systems with automatic alarms for the systems we have and also monitoring to ensure we are availible for our users. Those monitors have different alert levels and those neccesery to act on imidiatly will ensure Pager Duty alert the on-call person. The On-call person is expected to ensure that the issue is taken care of.

### Mobile app crashes
We are constantly monitoring the crash rate on our mobile apps and aim at haveing atleast 99.5% of our dayly app users to be crashfree. If this number drops below 99% it is considered an incident and shall be acted on accordingly. Meaning that the crash shall take pressence in priority. There shall be a post mortem to evaluating mitigations of root couse etc.

### Post Mortems
The person on-call or responsible to follow the incident is also responsible to ensure there is a post mortem of the incident after the urgent actions are taken. The point of the Post Mortem is to learn about what happened, share information, collect root causes for the issues, mitigate those, and make our way of working more resilient. We document all Post Mortems in [Google Drive] (https://drive.google.com/drive/folders/1VnXIj-JBJ3vFrclG8F6bHH0LJwH4Sh7g).
