# Root Cause Analysis

When facing production incidents we usually need quick mitigation to put out the fire and there is no time to deeply look at the underlying causes, treating symptoms and not the problem.

The goal of an RCA process is to discover the real cause behind the incident to fully understand how to solve it, prevent it in the future and have a record of successful strategies in order to share knowledge and repeat things that worked.

_Incidents could be defined as events that cause disruption to or a reduction in the quality of a production service or product feature which requires an emergency response._

In addition to discovering the root cause, we should strive to provide context and information that will result in an action or a decision: good analysis is actionable analysis.

The content on this repository should be shared once the incidents are mitigated or resolved so that potential vulnerabilities are not exposed.

In order to perform an Incident Analysis, you can choose the tool that better fits the situation, some common examples are: [5 Whys](https://en.wikipedia.org/wiki/Five_whys), [Fishbone Diagram](https://en.wikipedia.org/wiki/Ishikawa_diagram) (many potential causes, cause & effect) or [Change Impact Analysis](https://en.wikipedia.org/wiki/Change_impact_analysis)

Incidents Severity is categorized on the following levels:

- **SEV-1**: Critical issues impacting more than 50% of our users (a.k.a “Oh Fuck!”). The incident degrades the experience to a point in which the user decides to drop Decentraland Platform. Requires immediate resolution
- **SEV-2**: Critical system issue actively impacting a limited number of users. The users can still interact in Decentraland word but they get frustrated by the inability to live a full experience. Requires immediate resolution
- **SEV-3**: Stability or minor user impacting issue that requires immediate attention from the service owner, otherwise it might become a SEV-2 incident. Very restricted incident that is internally visible and should be mitigated as soon as possible; without extended user awareness and impacting non-critical flows
- **SEV-4**: Minor issue requiring action but not affecting the ability to use the platform
- **SEV-5**: Cosmetic issues or bugs not affecting the users’ ability to use the platform, but it's relevant to give awareness to the other teams

To add new incidents use the date of the event as the Id with the following format `YYYY-MM-DD`. If there is more than one event on the same date you may need to use a suffix as part of the file name.

---

## Incidents Index

- [2022-02-05](incidents/2022-02-05.md) Wearables not loading on some users backpack due to corrupted dropped wearable
- [2022-02-12](incidents/2022-02-12.md) CDN proxies stopped working affecting the ability to join Decentraland and some sites
- [2022-04-22](incidents/2022-04-22.md) Infura outage caused problem with different Services
- [2022-05-18](incidents/2022-05-18.md) Some issues were detected after the explorer release on
- [2022-06-06](incidents/2022-06-06.md) Social metrics tracking discrepancies
- [2022-07-12](incidents/2022-07-12.md) Catalyst node continuously rebooted after an update rollout
- [2022-07-25](incidents/2022-07-25.md) Cloudflare XSS protection prevented some users to deploy scenes or smart wearables
- [2022-08-02](incidents/2022-08-02.md) The Graph indexing delay prevented users from changing their wearables
- [2022-08-18](incidents/2022-08-18.md) Scenes not loading in Europe region
- [2022-09-01](incidents/2022-09-01.md) Users not able to save passport
- [2022-09-08](incidents/2022-09-08.md) Users not able to see or chat with each other
- [2022-10-17](incidents/2022-10-17.md) Some 3D models not rendering
- [2022-10-27](incidents/2022-10-27.md) Marketplace failed to display NFTs
- [2022-11-13](incidents/2022-11-13.md) Users joined to the #mvmf channel noticing huge lags
- [2022-11-15](incidents/2022-11-15.md) NFTs with animated gif thumbnails have stopped showing thumbnails
- [2022-11-17](incidents/2022-11-17.md) Changes in user profile not updating in peer perspective

## Vulnerabilities Index

- [2022-07-05](vulnerabilities/2022-07-05.md) Potentially outdated prices provided by the implementation of ChainlinkOracle
- [2022-07-06](vulnerabilities/2022-07-06.md) Take over of broken or expired Links
- [2022-07-13](vulnerabilities/2022-07-13.md) Arbitrary Modification content stored on S3
- [2022-07-20](vulnerabilities/2022-07-20.md) Cloudflare bypass for Biz environment
- [2022-08-11](vulnerabilities/2022-08-11.md) Broken access control when deleting single items
- [2022-08-12](vulnerabilities/2022-08-12.md) Subdomain takeover of osquery.decentraland.org
- [2022-08-23](vulnerabilities/2022-08-23.md) Stored XSS - Execute Malicious Javascript on Victim's Browser
