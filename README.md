# Introduction

The Fishbrain's Engineering Handbook is the central repository for knowledge and information for engineers in the organization. We aim to make this handbook accessible for everyone, as part of our effort to follow one of our main company values: Transparency and Honesty.

We welcome feedback. Please start a [pull request](https://github.com/fishbrain/engineering-handbook/pulls) to suggest improvements or to add clarifications. Please use [issues](https://github.com/fishbrain/engineering-handbook/issues) to ask questions.

## Sections

- [Quality](./Quality/README.md)
- [Fishway](./Fishway/README.md)


## Keeping yourself informed

To keep yourself up to date on everything going on in the company, as part of your onboarding, you will be made part of the following email lists and Slack channels. If this is not the case, please contact your manager.

* Email lists
	- Product team mailing list
	- Platform team mailing list
	- Engineering mailing list

* Slack
	- [#information](https://fishbrain.slack.com/archives/C0ARQHESJ)
	- [#everybody](https://fishbrain.slack.com/archives/C02FSLF41)
	- [#development](https://fishbrain.slack.com/archives/C029LM5J3)
	- [#bugs](https://fishbrain.slack.com/archives/C033QSRSN)
	- [#alerts](https://fishbrain.slack.com/archives/C9LPC3F25)

If you frequently check these channels, you can consider yourself informed.

### Other Related Pages

* [Fishbrain knowledge](https://docs.fishbrain.com/)
* [Fishbrain documentation](https://github.com/fishbrain/docs)

## On-Call

To scale our infrastructure we have a dev-ops culture including 24/7 support with rotating on-call. Conditions for this are documented in [Google Drive](https://docs.google.com/document/d/1vEP3QwE2EVNqQ6D7FjIIQAwhZe6pXnkfZQvt1vr7OAM/edit).


## Incident management

When we have an incident we must have a uniformed way of acting to them. This will reduce the load on the on-call person and ensure we do the right things at the time of the incident. 

If there is an incident it will be notified in the [#alerts](https://fishbrain.slack.com/archives/C9LPC3F25) channel on Slack and all dialogs about ongoing incidents shall be held there. If there is an outage or another need to get the attention of the on-call person there is a slack command "/pd trigger" that will fire a manual alert. Note that if the alert needs to reach the CTO it is done through PagerDuty and can be done by anyone on-call.

For all incidents that are impacting our users, it is important to share the information within Fishbrain in a transparent way so we can be proactive and honest with our users. Bigger incidents shall be shared in Slack [#everybody](https://fishbrain.slack.com/archives/C02FSLF41) and minor ones in [#support](https://fishbrain.slack.com/archives/CFDQ1DLSX).

### Security incidents
We have a documented security incident response plan that is used for any security and data incidents and details the work needed and the authorities that need to be informed in [Google Drive] (https://docs.google.com/document/d/1H5CvNvs6YesRPdjf2KcP4Vz2Z7nmpNOnJm_XB2dBWSU/edit).

### Backend failures

We have automatic alarms and monitoring setup for the systems we have to ensure Fishbrain is always available to our users. Those monitors have different alert levels and those necessary to act on immediately will ensure Pager Duty alert the on-call person. The On-call person is expected to ensure that the issue is taken care of.

### Mobile app crashes

We are constantly monitoring the crash rate for our mobile apps and aim at having at least 99.5% of our daily app users to be crash-free. If this number drops below 99% it is considered an incident and shall be acted on accordingly and the priority for resolving the crashes will take precedence. There shall be a post mortem to evaluate steps to mitigate the crash, find the root causes, etc.

### Post Mortems

The person on-call or responsible to follow the incident is also responsible to ensure there is a post mortem of the incident after the urgent actions are taken. The point of the post mortem is to learn about what happened, share information, collect root causes for the issues, mitigate those, and make our way of working more resilient. We document all post mortems in [Google Drive] 
