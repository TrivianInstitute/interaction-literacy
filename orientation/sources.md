# Sources, scope, and framework alignment

[Pathway](README.md) · Sources checked during drafting on 2026-10-11

The lessons combine short technical explanations, original fictional cases, and educational proposals. The primary sources below support the explanations within the stated scope. A cited publication does not endorse Trivian Institute or validate this pathway. No source is required reading to complete the offline activities.

Read a source for the particular claim at issue. Provider documentation describes mechanisms or an implementation perspective; it is not independent evidence that every product works as described. Risk frameworks identify concerns and practices; they do not estimate a risk's frequency in a given classroom. Research findings are limited by their design and setting.

## S1. Machine learning

**Google for Developers. [What is Machine Learning?](https://developers.google.com/machine-learning/intro-to-ml/what-is-ml).** Technical educational documentation.

Used in Lesson 1 for the relationship between data, training, predictions/classifications, and generated content. The pathway's everyday examples are newly written. The four activity labels are our teaching map and should not be represented as Google's taxonomy or a complete definition of AI.

## S2. Recommendation

**Google for Developers. [Recommendation systems overview](https://developers.google.com/machine-learning/recommendation/overview/types)** and **[Scoring](https://developers.google.com/machine-learning/recommendation/dnn/scoring)**. Technical educational documentation.

Used for candidate selection, scoring, ranking, and the effect of choosing a scoring objective. These sources explain common architectures and design considerations. They do not identify the current objectives of an unnamed platform or establish what a particular recommendation does to a person's wellbeing.

## S3. Language models

**Google for Developers. [LLMs: What's a large language model?](https://developers.google.com/machine-learning/crash-course/llm/transformers).** Technical educational documentation.

Used in Lesson 2 and the glossary for tokens, parameters, and a common form of language-model generation. The lesson deliberately leaves out architectural detail that a beginner does not need. The account should not be generalized to every kind of AI or used to settle claims about consciousness, creativity, or subjectivity.

## S4. Training and updating

**Google for Developers. [Production ML systems: Static versus dynamic training](https://developers.google.com/machine-learning/crash-course/production-ml-systems/static-vs-dynamic-training).** Technical educational documentation.

Supports distinguishing a training process from using a trained model, while recognizing different update arrangements. The lesson does not assume that every service has permanently fixed parameters. Whether a provider retains an interaction or uses it in later training is a separate, service-specific policy and implementation question.

## S5. Retrieval

**Lewis, P., and colleagues (2020). [Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks](https://arxiv.org/abs/2005.11401).** NeurIPS research paper; linked author manuscript.

Used to explain combining a generating model with retrieved external information. The paper evaluates particular RAG designs and tasks. It does not guarantee source accuracy, freshness, coverage, or faithful use of retrieved material in another implementation. The distinction between fetching a source and demonstrating how an answer used it is maintained in the worked case.

## S6. Application components

**Anthropic (2024). [Building effective agents](https://www.anthropic.com/engineering/building-effective-agents).** First-party engineering account.

Used as an architecture example in which a language model is combined with retrieval, memory, and external operations. It supports discussing a model and its surrounding application separately. The article notes that implementation details have changed since publication; the lessons make no current feature or performance claim about a named product. Neither action access nor saved memory should be inferred from conversational wording alone.

## S7. Generative-AI risks

**Autio, C., and colleagues, NIST (2024). [Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile](https://doi.org/10.6028/NIST.AI.600-1).** [Official PDF](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf).

Sections 2.2, 2.4, and 2.5 inform the bounded discussion of incorrect generated content, data privacy, and environmental variation. The document identifies risk categories and management considerations. It does not establish the prevalence of a failure in the fictional services or validate the lesson activities. No numerical footprint or universal resource cost is taken from it.

## S8. Data and bias

**Schwartz, R., and colleagues, NIST (2022). [Towards a Standard for Identifying and Managing Bias in Artificial Intelligence](https://doi.org/10.6028/NIST.SP.1270).** [Official PDF](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1270.pdf).

Used in Lesson 3 to distinguish data and computational questions from human and systemic sources of bias. The small fictional registration table illustrates an inference problem; it supplies no measured disparity, causal result, or population estimate. A larger dataset can still leave the wrong objective or an exclusionary process unexamined.

## S9. Accessibility

**World Wide Web Consortium, Web Accessibility Initiative. [Accessibility Principles](https://www.w3.org/WAI/fundamentals/accessibility-principles/).** Primary accessibility guidance.

Supports concrete examples involving keyboard operation, time, text alternatives, and perceivable/operable/understandable content. This lesson is an introductory educational application, not a WCAG conformance audit. Its participation options should be checked with learners and adapted; stating an option is not evidence that it meets everyone's needs.

## S10. Work

**Gmyrek, P., and colleagues, International Labour Organization (2025). [Generative AI and Jobs: A Refined Global Index of Occupational Exposure](https://www.ilo.org/publications/generative-ai-and-jobs-refined-global-index-occupational-exposure).** ILO Working Paper 140; [DOI](https://doi.org/10.54394/HETP0387).

Used for a task-level view of potential occupational exposure. Exposure estimates concern possibilities for tasks; they are not observed job-loss counts. River House's staffing questions are original design questions and make no forecast about that fictional center or a real employer.

## S11. Energy and material infrastructure

**International Energy Agency (2026). [Key Questions on Energy and AI](https://www.iea.org/reports/key-questions-on-energy-and-ai).** [Executive summary](https://www.iea.org/reports/key-questions-on-energy-and-ai/executive-summary).

Provides current institutional analysis of data-center electricity, infrastructure, supply chains, and opportunities and constraints in applying AI to energy systems. It supports treating digital activity as part of a physical setting. Global or regional estimates cannot establish a single service's footprint. Questions about equipment maintenance and disposal are proposed parts of a fuller lifecycle inquiry, not quantified findings about the fictional case.

## Framework alignment

### Sources used for the alignment

- **OECD/European Commission (2026). [Empowering Learners for the Age of AI: An AI Literacy Framework for Primary and Secondary Education](https://www.oecd.org/en/publications/empowering-learners-for-the-age-of-ai_65cd27d4-en.html).** Final publication, 18 June 2026; [DOI](https://doi.org/10.1787/65cd27d4-en). The final framework uses the domains **Engage with AI, Create with AI, Manage AI, and Shape AI**. This replaces reliance on the May 2025 review draft for this pathway's alignment note.
- **Cosgrove, J., and Cachia, R. (2025). [DigComp 3.0: European Digital Competence Framework — Fifth Edition](https://publications.jrc.ec.europa.eu/repository/handle/JRC144121).** Published 27 November 2025; [DOI](https://doi.org/10.2760/0001149). Its integration of AI across digital competence informs attention to digital information, participation, responsible use, wellbeing, and the environment.

### An interpretative connection, not a coverage certificate

| AILit domain | Connection in this beginner pathway | Where learning continues |
| --- | --- | --- |
| Engage with AI | Recognize described functions; question information, data, and wider effects. | Existing Interaction Literacy framing and verification modules. |
| Create with AI | Distinguish generated material from evidence and keep a reasoned revision visible. This offline pathway prepares for creative collaboration; it does not claim a full hands-on creation sequence. | [Embodied Creative Writing](https://github.com/TrivianInstitute/embodied-creative-writing). |
| Manage AI | Identify preparation versus action, permission changes, review, and correction. | Existing delegation module and [Interactive Dialogue](https://github.com/TrivianInstitute/interactive-dialogue). |
| Shape AI | Propose changes to a system's objectives, access routes, and accountability. This is introductory design participation, not completed technical model-building competence. | [Educator Commons](https://github.com/TrivianInstitute/educator-commons) and collaborative inquiry into further design work. |

DigComp 3.0 offers a complementary connection to wider digital literacy. The [Embodiment Commons](https://github.com/TrivianInstitute/embodiment-commons) extends inquiry into everyday digital conditions and embodied participation. This short orientation does not cover every competence in either framework, map to a certified proficiency level, or demonstrate age-specific learning outcomes. Adapting a primary/secondary framework for this older-learner and adult pathway requires educational judgment and evaluation.

## Keeping the evidence current

When a source changes, check the particular claim and update this note with the date and reason. Keep fictional scenarios distinct from field reports. Useful review questions include whether learners can distinguish the information layers, whether the lesson timings are realistic, which access barriers remain, and whether learners transfer the questions to another case. The existing [Learning in Practice](https://github.com/TrivianInstitute/learning-in-practice) framework supports appropriately bounded teaching feedback.
