## Quality

Quality is everyone's responsibility! Everything you merge to master should be production ready.

Appstore/Playstore reviews is the most important factor of the impression of our product and quality is mirroring those numbers. 
As a company we are striving for always reaching a score of **4.5** and if we are going below that number we need to increase the quality and customer focus ensuring that we are providing valuable functionality to the users.


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

To help ensure we adhere to this agreement we have a dashboard in [JIRA](https://fishbrain.atlassian.net/secure/Dashboard.jspa?selectPageId=10206) . In addition there is a weekly review of bugs older then 3 weeks to validate that the issues older are acted on in a timely manner and assigning issues where the team is not set.

### Crashes/Errors 
- Mobile apps

Crashes in the mobile apps are tracked in Firebase by Crashlytics. We treat all crashes as bugs and prioritize it according to the bugs. Our aim is to be above **99.5%** crash rate. If the Crash rate drops below **99.0%** it is considered an incident and shall be acted on with equal urgency.

- Web app

Errors on the web [are tracked in Bugsnag](https://github.com/fishbrain/mykiss-web/blob/develop/docs/frontend-guidelines/error-monitoring.md). [The current SLOs for the web](https://github.com/fishbrain/mykiss-web/blob/develop/docs/frontend-guidelines/slos.md) are a release stability of **99.9%** and **99.9% Uptime** in a time window of 7 Days.

- Backend

For backend services, the majority report errors to Bugsnag (including Rutilus). [The current SLOs for backend](https://docs.google.com/document/d/1GdoIj4CzLlZlAJTS9rTE9jIH52GL61qM-Lk0MpiVvyY/edit?ts=5dde8264) are that the error rate should be **<0.005%** measured per controller per hour, and that we have an uptime of **>99.5**.

### Loading times

- Mobile apps

Both [Google](https://developer.android.com/topic/performance/vitals/launch-time) and Apple [1](https://developer.apple.com/documentation/xcode/improving_your_app_s_performance/reducing_your_app_s_launch_time),[2](https://developer.apple.com/videos/play/wwdc2016/406/) provide with guidelines around app startup time. We are striving towards following the best practices and keeping loading times below the thresholds provided by the respective platforms.
Metrics around app loading times exist [here for Android](https://play.google.com/apps/publish/?account=8673675864021351303#AppHealthOverviewPlace:p=com.fishbrain.app&appid=4973867529686371805&aho=APP_HEALTH_DETAILS&ts=THIRTY_DAYS&ahbt=_CUSTOM). For iOS we are printing metrics in every run.

### Network performance

- Mobile apps

Firebase offers statistics around network performance of mobile clients and this is what we are tracking from the mobile apps side. Here is [Android](https://console.firebase.google.com/project/fishbrain.com:api-project-10207772235/performance/app/android:com.fishbrain.app/network) and here is [iOS](https://console.firebase.google.com/project/fishbrain.com:api-project-10207772235/performance/app/ios:com.fishbrain.app/network)


- Web

TBD


- Backend

TBD

### Critical app areas

We are striving towards high quality in the Fishbrain app as a whole. However some core areas of the app have a significant value for the user experience in Fishbrain.

The quality in those areas is prioritised and tested continuously for every new version of the apps through the UATs for both apps
- Account creation / Login
- Pro benefits
- New catches/Posts and their privacy
- Push Notifications
- Feed
- Fishbrain Shop


[Back to index](./../README.md)
