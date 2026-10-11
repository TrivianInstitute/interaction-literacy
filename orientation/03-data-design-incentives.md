# 03 — Data, design, and incentives

[Pathway](README.md) · [Previous lesson](02-from-training-to-answer.md) · [Next lesson](04-ai-in-a-shared-world.md) · 25 minutes

**Learning goal:** identify how data selection and a design objective can affect a recommendation, distinguish evidence from assumptions, and choose what information a task actually needs.  
**Materials:** this page and a way to make notes; no accounts or personal records.  
**Your artifact:** a revised recommendation design, a data boundary, and a reason to revise again.

## Whose idea of success? — 3 minutes

**Fictional situation:** Common Ground runs community classes. Its team asks a recommendation service to help residents find a suitable class. The provider reports success using the number of registration links opened. The center wants people to find classes they can attend and value.

Are those two measures asking the same question? Identify a situation where they might agree and one where they might diverge. All people, organizations, records, and outcomes in this lesson are fictional.

## Three design choices — 6 minutes

**Data is a selected record of a situation.** The examples collected, the categories used, and the people represented can affect the patterns a model learns or the information an application retrieves. A missing group, an inaccurate label, and an inappropriate decision rule are different problems. NIST's bias guidance examines computational, human, and systemic sources; adding more records alone does not settle every fairness question. [NIST SP 1270](sources.md#s8-data-and-bias).

**An objective is what a process is trained or configured to favor.** In recommendation, selecting a scoring objective affects which items appear first. For example, maximizing clicks can favor a different list from one designed around another outcome. This does not tell us the objective of a particular service; it gives us a question to investigate. [Google, recommendation scoring](sources.md#s2-recommendation).

**An incentive is a reason an organization or person may favor one outcome.** Revenue, access, learning, cost, and staff workload may create different priorities. The same service can balance several objectives. Do not infer a hidden motive just because a recommendation is poor; inspect the stated measures and the available evidence.

As a practical design choice, ask what information is necessary before sharing it. A task can sometimes be framed with preferences and constraints instead of identifying histories. Data protection also concerns retention, access, and reuse, not only the initial upload. NIST recognizes risks from unauthorized disclosure and from inferring sensitive information. [NIST's generative-AI profile, section 2.4](sources.md#s7-generative-ai-risks).

## Worked example: the registration record — 4 minutes

Common Ground supplies this fictional snapshot. It is a small teaching example, not a representative dataset or a model evaluation.

| Information available | What it supports | What remains unknown |
| --- | --- | --- |
| The recommendation service has last month's online registrations. | It has a record of some completed online choices. | Who wanted a class but could not register, and why. |
| Walk-in and telephone registrations were stored elsewhere. | The supplied source excludes those records. | Whether including them would change recommendations, and by how much. |
| Most entries in the supplied list are for morning classes. | Morning classes are common in this list. | Whether residents generally prefer mornings or only morning classes were well represented. |
| The provider ranks suggestions using predicted link openings. | The ranking targets that stated behavior. | Whether a high-ranking suggestion fits someone's schedule, access needs, or learning goal. |

A weak conclusion is, “Residents prefer mornings, so offer fewer evening classes.” The records do not establish that preference. A stronger first step is to ask what opportunities residents actually had, compare permitted information across registration routes, and invite feedback from people the online list misses.

That is a proposed investigation. We have not demonstrated that a particular change will improve participation. We can still make a concrete design revision: show time and access information, permit browsing the whole list, and assess suitability separately from link openings.

## Your task: redesign the recommendation — 8 minutes

Use the following invented request: “I want a beginner creative class next month, on an afternoon, with a step-free route. I do not want to create an account.” The center has verified class schedules and venue access descriptions. It has no information about the learner's identity or diagnosis.

Make a brief proposal that answers five questions:

1. **Define success.** What should a useful recommendation help this person do? Name a way to check it that does not equate popularity or clicks with suitability.
2. **Inspect representation.** Name one missing perspective in the online registration snapshot and a respectful way to investigate it. Avoid inventing what the missing people would say.
3. **Choose inputs.** Which details in the request are relevant? Which additional details should the system avoid demanding? Explain why a diagnosis is not needed to match a stated access requirement.
4. **Preserve choice.** Propose a way to see alternatives or correct a recommendation without an account. Who can fix an inaccurate venue description?
5. **Test a revision.** State one observation that would make you change your proposal. This may concern access, suitability, privacy, or workload.

Now change one fact: the center says its afternoon classes are full. Revise your response without silently removing the person's preferences. Would you offer a waitlist, another provider, a later date, or a direct conversation? You may reasonably propose more than one route.

Optional comparison within the same time: one learner represents the resident's priorities, another the staff's capacity, and a third the provider's design choices. Each should name a possible benefit and a limit of their own proposal. Independent work is equally valid.

## Feedback to compare — 3 minutes

A strong response could ask whether the person can identify an available class that fits their stated constraints, with optional feedback rather than compulsory tracking. It could compare online and other registration routes without collecting identifiable narratives. It could use preferred time, topic, skill level, and access requirement while avoiding names, medical history, or a complete activity log.

For correction, it might give a direct contact for the center's access-information owner and keep a plain-text or telephone route available. An observation such as “the step-free route information is inaccurate” should prompt verification and correction; “few people clicked” does not by itself explain why.

When classes are full, “nothing is available here at that time” is more defensible than redefining an unsuitable morning class as the best fit. Offering a later date or another provider can be reasonable. If the learner chooses a different route, assess whether the stated constraints and uncertainty remain visible.

Common omissions are assuming a group is represented because it could theoretically use a website, calling a metric a person's true preference, and collecting sensitive details without a task-based reason. Revise one omission rather than adding a longer request to the system.

## Exit and facilitation — 1 minute

Finish: “A measure can improve while the person's experience worsens when ___.” Name a concrete example from the fictional case.

Facilitators: let learners use fictional roles throughout. Do not inspect account settings or ask anyone to explain their own access needs. Offer an oral or drawn design. A person may favor an AI-assisted service, a simpler directory, or a staffed route; the reasoning and workable conditions are the learning evidence.

For attention and habit questions raised by ranking and interface design, continue into [Embodied Digital Life](https://github.com/TrivianInstitute/embodiment-commons/tree/main/courses/embodied-digital-life). The present lesson makes no claim about a particular design changing a person's brain.
