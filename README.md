Skype for Business Monitoring V2.2
==================================

V2.2 brings many hours of tweaking and polishing. The end result is a more stable, user friendly application that can be deployed in under 10 minutes. That's including watching my how to video!

#Why is it useful?
There are many different schools of thought around how best to monitor environments. Some folks are drawn to the physical aspects and tend to monitor processing, memory and disk. While this is useful information, its hardly sufficient on its own as an acceptable monitoring solution for Lync\Skype for Business. On the other hand, keeping a close eye on services and event logs can be most useful as well. This can lead to lots of verbose information and, on its own, monitoring services and events don't quite form a complete solution. My thinking involves generating traffic by means of synthetic transactions. It also involves a proactive approach rather than being reactive.

##For example:-
If you cant send an IM from user A to user B then its broken, regardless of it being a physical resource issue, a stopped service, certificate expiration or some other issue we have yet to uncover. The fact that the IM attempt is failing is sufficient to get my attention and subsequent action.

##Another example :-
If your test user cant make a PSTN call to a number of your choosing then there is a problem. Regardless of the true source of that problem (which will likely require an engineer). Be it monitoring service issue, SIP\PSTN issue from the provider or an issue with the SBC. It doesn't really matter..Why? because the issue has alerted me and I am now looking at it.

#What is this package?
It consists of two primary modules:-

1. Skype Monitoring Tool - This allows you to run a selection of synthetic transactions against any Skype Front End Pool on a frequency of your choosing
2. Monitoring Report App - This part monitors the results of the Skype Monitoring Tool, generates an alert email when tests fail and can also send daily and\or weekly reports of the test trends

##Functions
The results of each synthetic transaction are recorded in the Event Log of the PC where the tool is running.
The Event ID’s represent both success and failure of tests with separate ID’s depending on the result.
Event ID’s also contain a brief description of the test being performed, and in some cases a hint to resolution.
The tool also has a Schedule tab that will setup a scheduled task to run the synthetic transactions on a repetition interval of your choice.
Any test failures can generate an Alert Email so that you can proactively address the problem
Instead of trying to replace your existing monitoring tools, this tool generates Event Logs you can simply add to your monitored stack.

##What's been added in version 2.2?
UI improvements
bug fixes
Added an option for MONTHLY reports
Added an option for CUSTOM reports
Check out my blog at www.UCSorted.com for more information.

DISCALIMER This tool is NOT a replacement for the commercially available tools such as Nectar, EventZero or Prognosis. If you are after statistical data and history, triggered actions, dashboards, network performance, Session Border Controller monitoring or even QoS and network monitoring etc. then please do spend the cash and talk to these folks.
