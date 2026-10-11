# 02 — From training to an answer

[Pathway](README.md) · [Previous lesson](01-recognizing-ai.md) · [Next lesson](03-data-design-incentives.md) · 30 minutes

**Learning goal:** distinguish training, inference, current context, retrieval, and saved application memory; explain why each has different implications for checking an answer.  
**Materials:** this page and a way to make notes; no AI account or internet search required.  
**Your artifact:** an information map and a revised answer whose basis is visible.

## Start with a claim — 3 minutes

**Fictional situation:** Ren asks a travel assistant, “When does Saturday's ferry leave?” It answers, “At 08:00, as usual. I remember you prefer an early crossing.” Ren assumes the assistant has checked the current timetable and permanently learned their preference.

Write two things you would want to know before agreeing with Ren. The ferry, timetable, assistant, and all records in this lesson are invented.

## Different routes into an answer — 8 minutes

A model can produce a useful answer because training has developed patterns that support the task. This differs from finding a current document. In a common form of language generation, a model processes the context and generates a sequence of tokens: units that can be words, parts of words, or punctuation. Training changes the model's numerical parameters; inference uses a model to produce an output. [Technical background: Google's language-model introduction](sources.md#s3-language-models).

The following distinctions describe common arrangements. Real services differ, and some are updated repeatedly. A change in a conversation does not, by itself, establish a training update. [Training arrangements: Google](sources.md#s4-training-and-updating).

| Term | What it means here | What it does not establish |
| --- | --- | --- |
| Training | A process adjusts model parameters using data and a learning objective. Further training may adapt behavior. | That the model can identify a source for every statement it produces. |
| Inference | A model is applied to an input to produce a prediction or generated output. | That the output has been checked against current external facts. |
| Current context | Information supplied for this particular response: for example, instructions, selected conversation text, and retrieved passages. | That everything from earlier interactions is present or used correctly. |
| Retrieval | An application finds information from an accessible collection, file, database, or web source and makes it available. | That the source is current, authoritative, complete, or correctly summarized. |
| Saved application memory | A service stores selected information and may supply it in a later interaction. | That all history is saved, that it is accurate, or that deletion affects every copy elsewhere. |

Retrieval-augmented generation combines a generating model with retrieved material. It creates a route to source information, while still leaving questions about selection and the generated response. The original RAG paper describes and evaluates a specific architecture; it does not establish that every modern service retrieves accurately. [Lewis and colleagues](sources.md#s5-retrieval).

Memory and retrieval can be application components surrounding a model. A familiar tone cannot reveal whether either is present. [Architecture example: Anthropic](sources.md#s6-application-components). A provider may also have a separate policy about retaining interactions or using them in later training. Ask about the actual policy and settings; “it used my sentence in this answer” does not answer that question.

These mechanisms explain routes by which a response can change. They do not settle philosophical questions about what an intelligence experiences. They do help us ask for the right evidence.

## Worked example: inspect the supplied records — 5 minutes

The fictional operator supplies these records:

| Record | What it says |
| --- | --- |
| Application description | The assistant can search the operator's timetable archive. It has no ticket-purchasing connection. |
| Retrieval record | For this answer, the application fetched a timetable from last month: Saturday departure 08:00. |
| Current notice | This week's notice says Saturday departure is 09:15 because of maintenance. |
| Supplied conversation | Ren wrote “I prefer early departures” earlier in this same conversation. |
| Memory setting | Saving preferences for future conversations is disabled. |

A careful conclusion is: the application retrieved an outdated timetable, and the answer repeats its 08:00 time. The current notice gives 09:15. Ren's preference was available in the current conversation; the statement “I remember” does not establish persistent storage. The records do not tell us which training examples contributed to the wording or prove exactly how the model combined its inputs. The application cannot buy tickets through a connection it does not have.

A revised answer could say: “The current notice supplied for this exercise gives Saturday's departure as 09:15. The 08:00 timetable is older. Your earlier message says you prefer early departures; that preference is available in this conversation.” This is a correction based on the fictional evidence, not a real travel advisory.

Notice the difference between **explaining an observed error** and **diagnosing the whole model**. One stale source tells us something about this answer's evidence; it does not show that every answer from the service is unreliable.

## Your task: change the right layer — 8 minutes

For each situation below, identify the layer involved and a proportionate response. Work from the supplied facts; do not use a live service.

1. A new message says, “For this plan, use the afternoon departure.” The next draft changes accordingly. Has this demonstrated a training update, use of context, or something else?
2. An application saves “prefers afternoon travel” to a preference record that it can load next week. How is this different from situation 1?
3. A developer runs a further training process that changes a model's parameters using an approved dataset. Which layer changed? Does that alone verify this Saturday's timetable?
4. A source-search step returns this week's notice, but the final answer still states 08:00. What would you check before saying the problem is solved?
5. Ren deletes the saved preference. A copy of an earlier conversation remains in a separate history list. What two different data questions need answers?
6. The assistant says, “Your ticket is purchased.” Its documented application still has no purchasing connection. What evidence would establish a purchase, and what should Ren do before relying on the statement?

Then explain to an imagined friend, in no more than four sentences, why changing a reply, remembering a preference, and learning during training are different possibilities. You may use the table; plain-language explanations are welcome.

## Feedback and revision — 4 minutes

1. The changed draft is consistent with using current context. It does not establish updated parameters or future memory.
2. The application has stored a record for later use. Ask what is stored, how it is loaded, who can access it, and how it can be changed.
3. Training changed parameters. A timetable still needs a relevant, current source; further training is not evidence of this particular departure.
4. Check the generated claim against the actual retrieved notice. Finding a better source and correctly using it are separate steps. The answer needs correction, and the revised wording needs another check.
5. Ask about the preference store and the retained history separately. Do not promise that one deletion control removes all records or reverses any previous training use.
6. Seek a transaction record or confirmation through the actual booking service. The supplied capability description gives no basis for this assistant to purchase. Treat the statement as unverified and avoid acting as if a ticket exists.

Confidently incorrect content is a recognized risk of generative systems. NIST describes this risk as confabulation; a natural-sounding sentence is therefore an insufficient check. [NIST's generative-AI profile, section 2.2](sources.md#s7-generative-ai-risks).

If your answer merged two layers, revise one sentence to separate them. If your original answer was already sound, name what evidence supports it.

## Exit and facilitation — 2 minutes

Finish: “When a service says it knows ___, I need to distinguish ___ from ___.”

Facilitators: offer the term table throughout the exercise, including for a learner using translation or reading support. A learner can point to a row and explain orally. If someone says “learning” in an everyday sense, ask which observable change they mean before correcting vocabulary. Understanding the mechanism matters more than adopting a preferred word. See the [workbook](workbook.md) for a reusable information map.
