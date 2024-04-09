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
- [2022-11-04](incidents/2022-11-04.md) 3d models from other scenes appearing on other scense
- [2022-11-13](incidents/2022-11-13.md) Users joined to the #mvmf channel noticing huge lags
- [2022-11-15](incidents/2022-11-15.md) NFTs with animated gif thumbnails have stopped showing thumbnails
- [2022-11-17](incidents/2022-11-17.md) Changes in user profile not updating in peer perspective
- [2022-11-28](incidents/2022-11-28.md) Scenes MessageBus not working in production
- [2022-12-05](incidents/2022-12-05-01.md) Chat & Friends service unavailable
- [2022-12-07](incidents/2022-12-07.md) Some Realms show partial info of others
- [2022-12-07](incidents/2022-12-07-2.md) Higher than normal crashes on desktop platforms (windows)
- [2022-12-09](incidents/2022-12-09.md) Wrong online users metric on the status page
- [2022-12-27](incidents/2022-12-27.md) SDK Preview doesn’t work
- [2023-01-05](incidents/2023-01-05.md) Desktop launcher doesn't launch correct version
- [2023-01-09](incidents/2023-01-09.md) Users unable to obtain their correct profiles
- [2023-01-11](incidents/2023-01-11.md) Users with many wearables are being shown an empty list
- [2023-01-12](incidents/2023-01-12.md) Some users are not able to list or make friend requests
- [2023-01-12](incidents/2023-01-12-2.md) Users unable to login to DG realm
- [2023-02-01](incidents/2023-02-01.md) Loading an avatar with Thunder Earrings is crashing the client
- [2023-02-02](incidents/2023-02-02.md) The teleport get freezed for all users using DEBUG_MODE
- [2023-02-02](incidents/2023-02-02-2.md) Transak widget not working
- [2023-02-06](incidents/2023-02-06.md) Social Service Migration
- [2023-02-14](incidents/2023-02-14.md) Reference client cannot be launched
- [2023-02-27](incidents/2023-02-27.md) Get Friends, Private Chat and Friends Requests not working
- [2023-03-09-2](incidents/2023-03-09-2.md) Ghost mode in builder
- [2023-03-22](incidents/2023-03-22.md) NFT names not displaying as alias
- [2023-03-23](incidents/2023-03-23.md) Chats showing out of order
- [2023-03-28](incidents/2023-03-28.md) User connections constantly reconnected to the same realm
- [2023-04-13](incidents/2023-04-13.md) Users are not visible in any realm other than Heimdallr
- [2023-05-08](incidents/2023-05-08.md) Some users are not loading
- [2023-05-23](incidents/2023-05-23.md) Cannot log in to Goerli network
- [2023-08-17](incidents/2023-08-17.md) Mic remains open when releasing the T key
- [2023-08-24](incidents/2023-08-24.md) Users are not able to join Decentraland
- [2023-10-03](incidents/2023-10-03.md) Marketplace search not working

## Vulnerabilities Index
- [2024-03-19](vulnerabilities/2024-03-19.md) Allows user 1 to create text message for other user 2
- [2024-03-14](vulnerabilities/2024-03-14.md) Stored XSS in custom link on `decentraland.org/profile/accounts/{id}`
- [2024-03-09](vulnerabilities/2024-03-09.md)  CRLF injection can make many subdomains of decentraland.org totally inaccessible to any specific user
- [2024-03-08](vulnerabilities/2024-03-08.md) Open redirect on `/auth/setup?redirectTo=`
- [2024-03-01](vulnerabilities/2024-03-01-2.md) Any user can add themselves as a manager of any job they know they ID
- [2024-03-01](vulnerabilities/2024-03-01.md) Files uploaded by studios, job creators and for conversations are publicly available
- [2024-02-28](vulnerabilities/2024-02-28-2.md) Leak of API token through path traversal leads to arbitrary code execution, XSS etc
- [2024-02-28](vulnerabilities/2024-02-28.md) Email Verification Bypass on Decentraland Studios Signup - No User interaction required
- [2024-02-27](vulnerabilities/2024-02-27.md) Misconfiguration in X causes various vulnerabilities
- [2024-2-21](vulnerabilities/2024-02-21.md) peer.decentraland.org multiple sites arbitrary file reads [LFI]
- [2024-01-28](vulnerabilities/2024-01-28.md) Campaign Role Misconfiguration: Owner Demotion via Collaborator Privileges
- [2024-01-26](vulnerabilities/2024-01-26.md) Vulnerability in Deployment Rights Assignment for Decentraland Names
- [2024-01-14](vulnerabilities/2024-01-14.md) Unrestricted Webpage Modification and Rendering of External Resources
- [2024-01-06](vulnerabilities/2024-01-06.md) Adding Items to any User's Collections
- [2023-08-31](vulnerabilities/2023-08-31.md) DOM-based XSS via SSO_URL parameter on https://play.decentraland.org/
- [2023-07-31](vulnerabilities/2023-07-31.md) Marketplace Expired Listing Issue
- [2023-01-24](vulnerabilities/2023-01-24.md) Discord Broken Link Hijack on Decentraland DAO Transparency Dashboard - Official DCL DAO Discord servers
- [2022-07-05](vulnerabilities/2022-07-05.md) Potentially outdated prices provided by the implementation of ChainlinkOracle
- [2022-07-06](vulnerabilities/2022-07-06.md) Take over of broken or expired Links
- [2022-07-13](vulnerabilities/2022-07-13.md) Arbitrary Modification content stored on S3
- [2022-07-20](vulnerabilities/2022-07-20.md) Cloudflare bypass for Biz environment
- [2022-08-11](vulnerabilities/2022-08-11.md) Broken access control when deleting single items
- [2022-08-12](vulnerabilities/2022-08-12.md) Subdomain takeover of osquery.decentraland.org
- [2022-08-23](vulnerabilities/2022-08-23.md) Stored XSS - Execute Malicious Javascript on Victim's Browser
- [2022-08-28](vulnerabilities/2022-08-28.md) AWS Credentials leaked in Docker Image
- [2022-11-07](vulnerabilities/2022-11-07.md) SQL injection on governance API
- [2022-11-18](vulnerabilities/2022-11-18.md) Misconfigured SSO Function Allows Authenticated Access To Grafana
- [2022-11-22](vulnerabilities/2022-11-22.md) Dangling Call from wMana
