# 01 — Recognizing AI in everyday situations

[Pathway](README.md) · [Next lesson](02-from-training-to-answer.md) · 25 minutes · No AI account needed

**Learning goal:** identify what a described service does, distinguish an output from an action, and name what its appearance does not tell you.  
**Your artifact:** a function map with one uncertainty and a specific question that could resolve it.

## Begin with the experience — 3 minutes

**Fictional situation:** Harbor Library offers a service called Open Door. It puts three events at the top of a list, estimates which sessions will fill, writes a welcoming description, and offers to reserve a place. Its information card says its ranking, estimates, and descriptions use machine learning. Reservations are handled by a connected booking system.

Before reading on, describe the four activities in your own words. Which changes the information a person sees? Which could change an actual record? You can speak, write, draw four boxes, or think through the distinction privately.

## Four activities to recognize — 6 minutes

Machine learning is one approach to AI: a model is trained using data so it can make predictions or produce content in new situations. An AI service also includes choices about its interface, records, permissions, and use. A familiar-looking screen does not reveal how those components work. [Technical background: Google, introduction to machine learning](sources.md#s1-machine-learning).

The following labels are a teaching map, not four mutually exclusive kinds of intelligence. A service may combine them; prediction can be part of both ranking and generation.

| Activity | What to notice | An original example | A useful question |
| --- | --- | --- | --- |
| Ranking and recommendation | Some existing possibilities are selected or ordered for attention. | A class list places certain workshops first. | What makes something rank highly, and what is left out? |
| Prediction or classification | The system estimates a value or assigns a category. A prediction can concern a present condition, not only the future. | A model estimates attendance or labels a message as a booking question. | How accurate is it for this setting, and how are errors handled? |
| Generation | The system produces content, such as wording, an image, or audio. | A model drafts a workshop description. | Which parts require checking or attribution? |
| Delegated action | An application makes a change or communicates through a connected service. | It reserves a seat or sends an invitation. | What is it permitted to do, and who can review, stop, or correct it? |

Recommendation systems commonly select candidates and then score or reorder them. A high position reflects the system's selection process; it is not automatically a judgment of truth or suitability. [Technical background: Google's recommendation architecture](sources.md#s2-recommendation).

Action depends on the surrounding application and its connections. An explanation of a booking does not itself make a booking. Agentic applications can combine a language model with retrieval, storage, and external operations, but these capabilities should be checked for the particular system. [Architecture example: Anthropic](sources.md#s6-application-components).

## Worked example — 4 minutes

Open Door shows a pottery workshop first. That is ranking. The label “likely to fill soon” is a prediction. The paragraph beginning “Discover what your hands can make” is generated text in this fictional service. If selecting “Reserve” creates a booking in the library's records, that is action.

One plausible map therefore names all four activities. It also records an uncertainty: the page has not said whether the booking happens immediately or requires confirmation. A suitable question is, “What changes when I select Reserve, and is there a review screen before the record is created?”

The learner does not need to decide whether the service is good or bad before making this map. The map makes the decision more specific: useful event discovery can coexist with an unclear reservation step.

## Your task: map a mixed service — 8 minutes

**Everything on these six cards is fictional.** Use the facts on each card; do not assume additional capabilities.

| Card | Described behavior |
| --- | --- |
| A | A reading app uses a trained model to place five articles first, based on reading history. |
| B | A caption service generates words from an audio recording. A person can correct the transcript before publishing it. |
| C | A message service uses a trained classifier to mark a note “probably a request to reschedule.” It makes no calendar change. |
| D | A planning assistant drafts three event options, then sends the chosen option after a coordinator approves the recipients and wording. |
| E | A timer rings after the fixed number of minutes entered by its user. No other behavior is described. |
| F | A chat window says, “I have remembered your preference and booked the room.” No system record or capability description is supplied. |

For each card, name the activity or activities supported by the description. Add “uncertain” where needed. Choose one card and identify a plausible benefit, something that needs checking, and who could be affected. Finally, write one specific question that would resolve an uncertainty. “Is it safe?” is too broad; “Does this button send immediately?” is checkable.

## Compare your reasoning — 3 minutes

Read after making your own response.

- **A:** ranking/recommendation, supported by the description of a trained model. We do not know its objective or whether its recommendations are useful.
- **B:** generation; transcription can also be described as prediction over a sequence. Publishing is a separate action. Either technical description is acceptable if the learner distinguishes the draft from publication.
- **C:** prediction/classification. Labeling a message does not authorize changing an appointment.
- **D:** generation followed by an authorized communication step. The coordinator's review is part of the described workflow.
- **E:** the description establishes a fixed-rule timer. It provides no reason to infer a learned AI component. Ordinary automation and AI can coexist, but automation alone does not establish AI.
- **F:** the statement alone does not verify stored memory or an executed booking. Ask for the relevant record and the service's documented capabilities. An inaccurate completion claim is a possible explanation; so is a real action through an unseen integration. Preserve that uncertainty until checked.

An answer can use ordinary verbs such as “orders,” “estimates,” “writes,” and “sends.” The goal is a useful distinction, not memorizing labels. If you selected different categories, explain the overlap rather than forcing each card into one box.

## Exit and facilitation — 1 minute

Finish: “Before trusting this service with ___, I would check ___ because ___.” Keep the response for the [workbook](workbook.md).

Facilitators: read cards aloud or give them individually. Permit extra time, a partner to transcribe the learner's reasoning, or observing the comparison. Assess whether the learner identifies an activity and a real uncertainty. Do not use speed, willingness to create an account, or attitude toward AI as evidence of understanding.

[Continue: Where does an answer come from?](02-from-training-to-answer.md)
