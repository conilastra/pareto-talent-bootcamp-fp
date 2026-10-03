---
type: reference
title: Frontmatter standards
updated: 2026-10-03
---

```yaml
# every file
type: <company-overview | company | offer | icp | persona | testimonial | framework | market | competitor | competitor-lead-magnet | brand | funnel-asset | source | decision | log | moc>
title: ""
created: YYYY-MM-DD
updated: YYYY-MM-DD
sources: ["<source-note>", "https://..."]
tags: []
status: draft | verified | "[to be filled]"

# offer
price: ""
# persona
cause: ""
stage: ""
qualified: yes | no | depends
source_confidence: pareto-defined | candidate
# testimonial
client: ""
role: ""
right_hand: ""
result: ""
metric: ""
source_url: ""
# framework
taught: "Day N"
# competitor
website: ""
category: va-provider | staffing | marketplace | bpo | other
# competitor-lead-magnet
competitor: "<competitor-note>"
url: ""
format: ""
promise: ""
audience: ""
captures_with: ""
qualifies_by: ""
post_optin: ""
# funnel-asset
funnel_stage: TOFU | MOFU | BOFU | all
persona: "<persona-note>"
tool: ""
live_url: ""
# source
source_type: transcript | document | web-page
captured: YYYY-MM-DD
origin_url: ""
# decision
decided: YYYY-MM-DD
options_considered: []
reason: ""
```
