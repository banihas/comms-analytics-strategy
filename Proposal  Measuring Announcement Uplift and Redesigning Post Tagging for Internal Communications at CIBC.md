# Proposal: Measuring Announcement Uplift and Redesigning Post Tagging for Internal Communications at CIBC

## Overview

This proposal recommends two related improvements to internal communications measurement at CIBC:

- A defined method to quantify the impact (uplift) of Viva Engage announcements on reach and engagement.
- A redesigned tagging taxonomy for posts that replaces ad-hoc categories with a small, research-backed set of message types and attributes.

These changes will make portfolio KPIs more meaningful, help comms leaders use announcements intentionally, and provide clearer evidence on how different types of content perform across communities and portfolios.[^1][^2][^3]

## Current state and problem

### Announcements

Announcements in Viva Engage send push notifications to Outlook or Teams and are primarily used to increase the proportion of employees who see a post, especially for important messages.[^3][^1]

In practice, announcements:

- Almost always increase the percentage of the audience who see content (reach).
- Often lower engagement rate (reactions/comments per reached person) compared to non-announcement posts, because employees treat them as broadcast information rather than conversational content.

At present, this trade-off is understood informally but is not being measured systematically. That makes it difficult to answer questions like “Are we overusing announcements?” or “For which types of messages are announcements actually helpful?”[^2][^3]

### Post tagging

Post tags are currently based on locally defined categories and sub-categories created by comms leadership. These labels do not follow a shared taxonomy, and their definitions are not aligned with internal communications or content tagging best practices.[^4][^2]

The consequences are:

- Inconsistent tagging by authors.
- Limited ability to segment metrics by meaningful dimensions like message purpose, urgency, or audience.
- Difficulty comparing performance across portfolios and content types.

Industry guidance on content tagging and internal communications stresses the importance of a small, well-defined set of categories based on business-relevant dimensions such as message purpose, audience, and urgency.[^5][^4][^2]

## Objectives

This proposal aims to:

1. Quantify the impact of announcements on reach and engagement for each portfolio and message type.
2. Align post tagging with internal communications best practice so that KPIs reflect meaningful content dimensions.
3. Enable better decisions about when to use announcements and how to design communications for different objectives.

## Measuring announcement uplift

### Key metrics

The following metrics can be derived from Viva Engage analytics for each post:[^6][^7][^8]

- **Audience size (intended recipients):** Member count of the targeted community or segment.
- **People reached:** Unique employees who viewed, reacted to, or replied to the post.
- **People engaged:** Unique employees who reacted or commented.

From these, define three rates:

1. **Reach rate**

\(\text{Reach rate} = \frac{\text{people reached}}{\text{audience size}} \times 100\)

This measures what fraction of the intended audience saw the post. Internal communications guidance treats reach rate as a core KPI for announcements and intranet content.[^9][^10][^3]

2. **Engagement rate**

\(\text{Engagement rate} = \frac{\text{people engaged}}{\text{people reached}} \times 100\)

This is consistent with Viva’s "engaged breakdown"—the percentage of reached employees who interacted via reactions or comments.[^7][^8]

3. **Engaged audience share**

\(\text{Engaged audience share} = \frac{\text{people engaged}}{\text{audience size}} \times 100 = \text{Reach rate} \times \text{Engagement rate}\)

This shows what fraction of the total audience both saw and interacted with the post. Measurement frameworks for internal communications emphasize tracking not just reach and interaction but also the proportion of the audience that takes some action or shows deeper engagement.[^11][^12]

### Comparing announcement vs non-announcement posts

For any given portfolio, community, or message type, calculate post-level metrics for two groups:

- **Announcement posts:** Posts where the announcement feature was used.
- **Non-announcement posts:** Posts published without announcements.

Then compute summary statistics (median or mean) for each group over a defined period (e.g., one year):

- \(R_{\text{ann}}\): Reach rate for announcement posts.
- \(R_{\text{non}}\): Reach rate for non-announcement posts.
- \(E_{\text{ann}}\): Engagement rate for announcement posts.
- \(E_{\text{non}}\): Engagement rate for non-announcement posts.
- \(A_{\text{ann}}\): Engaged audience share for announcement posts.
- \(A_{\text{non}}\): Engaged audience share for non-announcement posts.

Using medians or trimmed means reduces the influence of a few unusually successful or unsuccessful posts, which internal communications analytics guidance recommends when comparing content performance.[^13][^14]

### Uplift and trade-off metrics

Define the following metrics to quantify uplift and trade-offs:

1. **Reach uplift**

- Absolute uplift (percentage points): \(\Delta R = R_{\text{ann}} - R_{\text{non}}\)
- Relative uplift (ratio): \(U_R = \frac{R_{\text{ann}}}{R_{\text{non}}}\)

This shows how much announcements increase reach compared to similar posts without announcements. For example, if non-announcement posts reach 60% of the audience and announcements reach 85%, then \(\Delta R = 25\) points and \(U_R \approx 1.42\), meaning a 42% relative uplift.[^9][^3]

2. **Engagement impact**

- Engagement delta: \(\Delta E = E_{\text{ann}} - E_{\text{non}}\)
- Engagement ratio: \(U_E = \frac{E_{\text{ann}}}{E_{\text{non}}}\)

In observed data, announcements generally lower engagement rate—employees are more likely to see the content but less likely to react or comment per viewer. Framing this explicitly as a delta and ratio makes the trade-off transparent.[^2][^3]

3. **Engaged audience impact**

- Engaged audience delta: \(\Delta A = A_{\text{ann}} - A_{\text{non}}\)

This metric captures whether announcements increase or decrease the fraction of the total audience that both sees and interacts with the message. Internal communications ROI discussions emphasize understanding not only who sees the message but who acts or engages, particularly for campaigns and mandatory communications.[^15][^11]

### Interpretation for decision-making

The combination of \(\Delta R\), \(\Delta E\), and \(\Delta A\) provides a structured way to decide when announcements are appropriate:

- For **critical or mandatory messages** (e.g., policy/compliance, major change, enterprise-wide leadership announcements), a positive \(\Delta R\) with a modest negative \(\Delta E\) is acceptable: the primary objective is awareness and compliance, not conversation.[^3][^9]
- For **culture, recognition, and engagement-focused content**, a large negative \(\Delta E\) and \(\Delta A\) indicate that announcements may be harming the community’s conversational engagement. In these cases, non-announcement posts or campaign-style communication may be better suited.[^16][^15][^2]

Reporting these metrics annually for each portfolio and message type will allow comms leaders to tune their use of announcements based on evidence rather than intuition.

## Limitations and safeguards

When measuring uplift, it is important to recognize that announcements are not randomly assigned; they are used more often for certain message types and tiers. This can introduce selection bias in the metrics.[^17][^15]

To mitigate this:

- Segment analysis by message type and tier (see tagging section below) so announcements are compared to similar non-announcement posts.
- Use multiple periods of data (e.g., year-over-year) to see whether patterns are consistent.
- Treat uplift metrics as directional evidence rather than strict causal estimates.

## Redesigning post tagging

### Why current tags are insufficient

Content tagging research emphasizes that tags should be designed around clear business purposes and user needs (discovery, personalization, analytics), not solely around locally invented labels.[^4][^5]

When categories and sub-categories are not tied to well-defined dimensions such as message purpose, audience segment, and urgency, several problems arise:

- Authors interpret categories differently, leading to inconsistent tagging.[^4]
- Analysts cannot reliably group posts into meaningful buckets for KPI calculations.
- It becomes difficult to answer questions like “How do change communications perform versus recognition posts in this portfolio?”

Improving tags therefore means grounding them in a small, research-backed taxonomy that mirrors how internal communications professionals describe content types and campaigns.[^18][^16][^2]

### Design principles for a better tagging system

Drawing from internal communications and content tagging best practices, the proposed tagging system adheres to four principles:[^5][^2][^4]

1. **Small, fixed set of primary types**

Use 6–10 message types that cover all content, with clear definitions and examples. This aligns with recommendations to keep tag sets concise and business-oriented.[^16][^5][^4]

2. **Separate dimensions for type, tier, audience, and format**

Avoid overloading a single field with multiple concepts. Instead, use distinct fields for message type, urgency/tier (critical vs FYI), audience segment, and optionally format. This approach mirrors tagging strategies that use separate tags for topic, audience, and format to support better discovery and analytics.[^5][^3][^4]

3. **Clear, mutually exclusive labels**

Tag names should be short and specific, and each tag should represent a single concept (e.g., “Policy & compliance” rather than “Policy/HR general”). This reduces ambiguity and increases consistency in author tagging.[^19][^4]

4. **Explicit definitions and examples**

Each tag should have a one-sentence definition and a small set of examples drawn from existing posts. Guidance from tagging and analytics platforms emphasizes the importance of documentation so users apply tags consistently.[^19][^4][^5]

### Proposed message type taxonomy

Based on common internal communications content types, the following message type taxonomy is recommended:[^18][^2][^16]

1. **Leadership & strategy**

- Definition: Messages from senior leaders (CEO, SBU leaders, executive committees) about strategy, performance, vision, or major organizational news.
- Examples: CEO quarterly update, SBU performance summary, enterprise-wide strategic announcement.

2. **Change & initiative**

- Definition: Communications announcing or explaining changes to organizational structure, tools, processes, or major initiatives that affect how employees work.
- Examples: restructuring notification, new technology rollout, transformation program launch.

3. **Operational update**

- Definition: Short-form updates about day-to-day operations, processes, systems, or schedules.
- Examples: IT maintenance notice, branch operating hours change, process update for frontline teams.[^18]

4. **Policy & compliance**

- Definition: Messages about policies, regulatory requirements, mandatory training, or risk and compliance guidance.
- Examples: AML policy update, mandatory training reminder, new HR policy announcement.[^2][^3]

5. **HR & benefits**

- Definition: Communications about compensation, benefits, wellness programs, and employee resources that are not strictly compliance notices.
- Examples: benefits enrollment campaign, wellness initiative, new employee assistance program.[^20][^2]

6. **Culture & recognition**

- Definition: Posts highlighting employees, teams, values, corporate social responsibility, and cultural initiatives.
- Examples: employee spotlight story, awards announcement, volunteer event recap.[^20][^16][^2]

7. **Learning & enablement**

- Definition: Messages promoting training opportunities, knowledge resources, and how-to guidance that help employees perform better.
- Examples: new training course announcement, how-to guide for a tool, curated knowledge packs.[^4][^2]

8. **Campaign**

- Definition: Structured, multi-touch communications with defined objectives, target audience, channel plan, timeline, and measurable outcomes.
- Examples: safety month campaign, diversity week, tool adoption campaign.[^15][^17]

These types line up with external internal communications guidance, which distinguishes leadership communications, change and operational updates, HR/policy content, and culture/recognition stories as distinct categories.[^16][^2][^18]

### Additional tagging dimensions

To support richer analysis and more intentional use of announcements, three additional tagging dimensions are recommended:

1. **Tier / urgency**

Inspired by intranet guidance that differentiates critical, important, and informational messages, introduce a tier field:[^3]

- Critical – Must-read, high-stakes, often compliance or crisis-related.
- Important – Strongly relevant but not immediate crisis-level.
- Informational / FYI – Contextual or cultural content; helpful but not mandatory.

This field provides a principled basis for deciding when announcements are appropriate: critical and some important messages may justify announcements; informational content generally should not.[^3][^18]

2. **Audience segment**

Use a controlled list of audience segments such as:

- Enterprise-wide.
- SBU (e.g., Retail Banking, Wealth Management).
- Function (e.g., Technology, HR).
- Region or location.

Tagging audience segments aligns with internal communications targeting guidance, which recommends using filters and segments to deliver relevant messages and to analyze impact by audience characteristics.[^21][^22][^18]

3. **Action intent**

Introduce a simple action intent field:

- Action required – Employee needs to do something (e.g., complete training, update information).
- Awareness – Employee needs only to be informed.

Labeling posts with action intent is recommended in internal communications and intranet best practices so employees can prioritize messages; it also enables analytics on how well action-required messages drive behaviors compared to awareness-only posts.[^18][^3]

4. **Format (optional)**

If not already captured elsewhere, add a format field:

- Short text, long-form article, video, image gallery, poll, etc.

Content tagging strategies often use format tags alongside type and audience so teams can analyze whether certain formats (e.g., video recognition posts) perform better for specific message types and audiences.[^5][^4][^3]

### How improved tags strengthen measurement

With the proposed tags in place, announcement uplift and engagement metrics can be analyzed at a more granular level:

- Compare reach and engagement for **change & initiative** messages with and without announcements, by tier and audience segment.
- Assess whether **culture & recognition** posts lose conversational engagement when announcements are used.
- Evaluate whether **action-required** messages achieve higher engaged audience share when supported by announcements, campaigns, or manager cascades.

Internal communications frameworks for campaigns emphasize tracking outcomes by content type, audience, and channel plan. A structured tagging system enables those analyses within Viva Engage data.[^17][^15][^18]

## Implementation roadmap

### Phase 1: Design and alignment (4–6 weeks)

1. **Validate the taxonomy with comms leadership**

Present the proposed message types, tier levels, audience segments, and action intent to comms leaders and gather feedback. Adjust labels and examples to fit CIBC’s language while preserving the underlying structure.[^2][^4]

2. **Document definitions and examples**

Create a short tagging guide with definitions, examples, and a decision flow (“If the message is from a senior leader about strategy, tag it as Leadership & strategy”). Documentation is a common recommendation for effective tagging systems.[^19][^4][^5]

3. **Update author workflows**

Integrate the new tags into authoring templates and training for comms staff and community owners. Emphasize that tags are measurement levers, not optional decorations.

### Phase 2: Data collection and baseline (3–6 months)

1. **Apply new tags to new posts**

Begin tagging all new posts with the redesigned taxonomy. Where feasible, backfill tags on recent high-importance posts to build a baseline.

2. **Extract and store Viva analytics**

Set up regular exports or access to Viva Engage analytics for post-level metrics (audience size, people reached, people engaged, announcement flag). Store these in a structured dataset keyed by community, portfolio, and tags.[^8][^6][^7]

3. **Compute initial uplift metrics**

For each portfolio and major message type, calculate \(R_{\text{ann}}\), \(R_{\text{non}}\), \(E_{\text{ann}}\), \(E_{\text{non}}\), \(A_{\text{ann}}\), and \(A_{\text{non}}\) for a baseline period.

### Phase 3: Reporting and decisions (ongoing)

1. **Annual portfolio KPI review**

In the annual review of each portfolio, include:

- Announcement reach uplift (\(\Delta R\) and \(U_R\)).
- Engagement impact (\(\Delta E\) and \(U_E\)).
- Engaged audience impact (\(\Delta A\)).

Break these down by message type and tier to provide actionable insight.

2. **Guidelines for announcement use**

Based on observed metrics, develop guidelines such as:

- Use announcements for critical and important messages where reach is the priority.
- Avoid announcements for culture & recognition posts where conversational engagement is more valuable.
- For campaigns, design channel plans that combine community posts, manager cascades, and selective announcements.

This approach mirrors best practices that distinguish one-off announcements from structured campaigns.[^15][^17][^18]

3. **Continuous improvement**

Review tag distributions and metric behavior annually. Adjust tag definitions or examples where confusion persists, and refine guidelines as data accumulates.

## Expected benefits

Implementing the measurement of announcement uplift and redesigning post tagging is expected to deliver several benefits:

- **Evidence-based use of announcements:** Leaders can see where announcements truly improve reach and where they unnecessarily suppress engagement.
- **More meaningful KPIs:** Portfolio KPIs for reach and engagement will be segmented by message type, tier, and audience, making them more useful for leadership conversations.
- **Better design of communications:** Comms teams can tailor formats, channels, and tagging based on how different content types perform in different portfolios.
- **Improved discoverability and governance:** Structured tags make content easier to find and reuse, and they support governance of internal communications by topic and audience, as recommended by intranet and tagging best practices.[^4][^2][^5][^3]

Overall, these changes move measurement from raw counts and ad-hoc labels toward a structured, evidence-driven framework aligned with internal communications practice.

---

## References

1. [8 Actionable Internal Communication Best Practices for 2025](https://www.guidejar.com/blog/8-actionable-internal-communication-best-practices-for-2025) - |Multi-Channel Communication Strategy|High: multiple platforms to manage|High: investment in tools a...

2. [Internal Communication Best Practices: 25 Ideas to Boost ...](https://www.exoplatform.com/blog/internal-communication-best-practices/) - - **Use Search and Tagging:** Enable robust search, categorization, and tagging to make content easy...

3. [www.happeo.com › blog › intranet-for-internalIntranet For Internal Communication - Happeo](https://www.happeo.com/blog/intranet-for-internal-communication/) - - **Measurable reach**: Unlike email, you can track who actually read critical announcements and fol...

4. [8 Practical Tips for Better Content Categorization](https://easycontent.io/resources/8-practical-tips-for-better-content-categorization/) - - Use audience, format, and purpose tags - these tags make content instantly discoverable and help t...

5. [Content Tagging Strategy: 90 Days to Govern AI Tagging](https://photofy.com/2026/10/11/content-tagging-strategy/) - - **Format**: video, image, blog post, carousel, and similar.
- **Audience**: who the content is mea...

6. [Monitor engagement in Viva Engage with analytics - Microsoft Support](https://support.microsoft.com/en-us/topic/monitor-engagement-in-viva-engage-with-analytics-0d9f6fd5-6b0c-45a2-a0aa-0576ae1f6895) - ||A count and charting pattern of people who viewed, reacted or commented on your posts.|
...
||The ...

7. [View community insights](https://support.microsoft.com/en-us/viva/engage/view-community-insights) - |**Engaged breakdown**|The percentage of people who engaged, by reacting or commenting.|

8. [Track engagement in Viva Engage with analytics - Microsoft Support](https://support.microsoft.com/fr-FR/viva/engage/vivaengage/track-engagement-in-viva-engage-with-analytics) - |**Engaged breakdown**|The percentage of people who engaged, by reacting or commenting.|

9. [KPIs for Internal Communications: The 7 Metrics You Must Track! - Vouch videos](https://www.vouchfor.com/blog/kpis-for-internal-communications) - If a company announcement reaches 650 employees out of an intended audience of 800, the reported rea...

10. [4 Smart Ways to Measure Your Internal Communication](https://haiilo.com/blog/4-smart-ways-to-measure-your-internal-communication) - - **Reach**: How many employees are you reaching?
- **Engagement**: How are employees engaging with ...

11. [How to Measure & Prove Internal Communications ROI](https://www.poppulo.com/employee-experience-platform/blog/internal-communication-roi) - The **employee engagement** and action rate measures the percentage of recipients who took the inten...

12. [cerkl.com › blog › internal-communications-measurement-frameworkThe 2026 Internal Communications Measurement Framework](https://cerkl.com/blog/internal-communications-measurement-framework) - That means tracking reach (deduplicated across every channel), engagement (who opened and read, by n...

13. [Internal Communication Metrics: 2026 KPI Guide - Jint](https://www.jint.co/internal-communication/internal-communication-metrics-kpis) - Engagement metrics get closer to the truth: read time, scroll depth, likes, comments, shares, and cl...

14. [Measuring internal communications](https://www.interactsoftware.com/blog/measuring-internal-communications-takeaways/) - |Engagement|Are they doing anything with it?|Comments, reactions, shares, dwell time, drop-off rates...

15. [Internal Communication Campaigns: Creative Strategies for ...](https://www.hubengage.com/feeds/blog/employee-engagement-internal-communication-campaigns) - Unlike reactive announcements or scattered emails, campaigns follow a structured approach with defin...

16. [8 Types of Internal Communication You Need to be Doing](https://www.wnccumc.org/resourcedetail/8-types-of-internal-communication-you-need-to-be-doing-18873631) - - Interest, buy-in, and engagement: ‘teaser’ campaigns that pique interest are a particular hit for ...

17. [How to Create Internal Communication Campaigns](https://www.hrcloud.com/blog/how-to-create-internal-comms-campaigns?hs_amp=true) - Unlike one-off announcements, a campaign has a defined objective, a target audience, a channel plan,...

18. [How to Create an Internal Communications Plan in 6 Steps - Workvivo](https://www.workvivo.com/es/internal-communications/plan/) - |Operational updates|Short-form announcement|Slack / Teams + intranet|

19. [Advice for AI Tags - WFO Help Center](https://wfohelp.com/doc/Content/user-guides/analytics/about-ai-tags.htm) - A **category** is a collection of tags that you organize together because they have a similar busine...

20. [20 Intranet Content Ideas to Boost Employee Engagement](https://clickup.com/blog/intranet-content-ideas/) - For large organizations, breaking content down into categories or themes (e.g., HR, IT, Marketing) c...

21. [How to target your internal communication? The 4 steps - Jint](https://www.jint.co/blog-posts/targeted-internal-communication) - In addition, these *tags* allow employees to subscribe to themes.

22. [Internal Communication Multi-Filters: Smart Targeting ...](https://www.cleverence.com/articles/sage-documentation/internal-communication-multi-filters-4827/) - Instead of selecting a single attribute like department, you combine multiple attributes - such as d...

