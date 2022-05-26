# Root Cause Analysis

When facing production incidents we usually need a quick mitigation to put out the fire and there is no time to deeply look at the underlying causes, treating symptoms and not the problem. 

The goal of an RCA process is to discover the real cause behind the incident to fully understand how to solve it, prevent it in the future and to have a record of successful strategies in order to share knowledge and repeat things that worked. 

*Incidents could be defined as events that causes disruption to or a reduction in the quality of a production service or product feature which requires an emergency response.*   

In addition to discovering the root cause, we should strive to provide context and information that will result in an action or a decision: good analysis is actionable analysis.

The content on this repository should be shared once the inicidents are mitigated or resolved so that we don't expose potential vulnerabilities.

In order to perform an Incident Analysis you can choose the tool that better fits the situation, some common examples are: [5 Whys](https://en.wikipedia.org/wiki/Five_whys
), [Fishbone Diagram](https://en.wikipedia.org/wiki/Ishikawa_diagram) (many potential causes, cause & effect) or [Change Impact Analysis](https://en.wikipedia.org/wiki/Change_impact_analysis)

--- 

## Incidents Index

- [Incident-1](Incidents/incident-1.md) *Feb-07-2022* Wearables not loading on some users backpack due to corrupted dropped wearable
- [Incident-2](Incidents/incident-2.md) *Feb-13-2022* CDN proxies stopped working affecting the ability to join Decentraland and some sites
- [Incident-3](Incidents/incident-3.md) *Apr-22-2022* Infura outage caused problem with different Services
- [Incident-4](Incidents/incident-4.md) *May-18-2022* Some issues were detected after the explorer release on May-18-2022