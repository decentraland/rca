# Root Cause Analysis

When facing production incidents we usually need a quick mitigation to put out the fire and there is no time to deeply look at the underlying causes, treating symptoms and not the problem. 

The goal of an RCA process is to discover the real cause behind the incident to fully understand how to solve it, prevent it in the future and to have a record of successful strategies in order to share knowledge and repeat things that worked. 

*Incidents could be defined as events that causes disruption to or a reduction in the quality of a production service or product feature which requires an emergency response.*   

In addition to discovering the root cause, we should strive to provide context and information that will result in an action or a decision: good analysis is actionable analysis.

The content on this repository should be shared once the incidents are mitigated or resolved so that potential vulnerabilities are not exposed.

In order to perform an Incident Analysis, you can choose the tool that better fits the situation, some common examples are: [5 Whys](https://en.wikipedia.org/wiki/Five_whys
), [Fishbone Diagram](https://en.wikipedia.org/wiki/Ishikawa_diagram) (many potential causes, cause & effect) or [Change Impact Analysis](https://en.wikipedia.org/wiki/Change_impact_analysis)

Incidents Severity are categorized on the following levels: 

- **SEV-1**: Critical issues impacting more than 50% of our users (a.k.a “Oh Fuck!”). The incident degrades the experience to a point in which the user decides to drop Decentraland Platform. Requires immediate resolution
- **SEV-2**: Critical system issue actively impacting a limited number of users. The users can still interact in Decentraland word but they get frustrated by the inability to live a full experience. Requires immediate resolution
- **SEV-3**: Stability or minor user impacting issue that requires immediate attention from the service owner, otherwise it might become a SEV-2 incident. Very restricted incident that is internally visible and should be mitigated as soon as possible; without extended user awareness and impacting non-critical flows
- **SEV-4**: Minor issue requiring action but not affecting the ability to use the platform
- **SEV-5**: Cosmetic issues or bugs not affecting the users’ ability to use the platform, but it's relevant to give awareness to the other teams

To add new incidents use the Date of the event as the Id with teh following format `YYYY-MM-DD`. If there is more than one incident on the same date you may need to use a suffix as part of the file name.

--- 

## Incidents Index

- [2022-02-05](incidents/2022-02-05.md) Wearables not loading on some users backpack due to corrupted dropped wearable
- [2022-02-12](incidents/2022-02-12.md) CDN proxies stopped working affecting the ability to join Decentraland and some sites
- [2022-04-22](incidents/2022-04-22.md) Infura outage caused problem with different Services
- [2022-05-18](incidents/2022-05-18.md) Some issues were detected after the explorer release on 
- [2022-06-06](incidents/2022-06-06.md) Social metrics tracking discrepancies
- [2022-07-12](incidents/2022-07-12.md) Catalyst node continuously rebooted after an update rollout
- [2022-08-02](incidents/2022-08-02.md) The Graph indexing delay prevented users from changing their wearables


