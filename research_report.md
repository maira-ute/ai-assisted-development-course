# Applications of Generative AI: Benefits, Challenges, and Real-World Examples

**Research report**

**Focus:** Cross-industry applications, with emphasis on geographic information systems (GIS)

**Prepared:** November 2026

## Executive Summary

Generative artificial intelligence (GenAI) creates new content—such as text, images, software code, audio, video, or structured data—in response to a prompt or other input. It can help people work with information faster, create first drafts, and interact with complex systems in natural language. In GIS, these abilities can make geospatial data and tools more accessible: users can ask questions about Earth-observation data, draft analysis scripts, summarize spatial results, and produce map descriptions.

These systems do not guarantee that generated content is true, complete, safe, or geographically correct. Their output needs to be checked against authoritative data and domain expertise, especially when it could affect health, public safety, land use, or resource allocation. The most useful deployments treat GenAI as an assistant in a human-led workflow, not as an independent source of truth.

## What Counts as Generative AI?

Generative AI models learn patterns from data and use them to generate new outputs. Large language models (LLMs) generate text and code; image models generate or edit visual content; multimodal models can work across text, images, audio, and other inputs. A system may also use retrieval-augmented generation (RAG), which searches selected documents or databases and supplies relevant material to a language model before it answers.

Not every system described as “AI” is generative. For example, a model that classifies satellite images or predicts flood risk may be valuable AI without generating content. This distinction matters in GIS, where established machine-learning methods already support mapping, classification, and forecasting. GenAI can complement those methods—for instance, by helping a user formulate a query or explain a model’s output—but should not be assumed to replace them.

## Applications and Examples

### GIS and Earth Science

GenAI can make geospatial data catalogs and GIS tools easier to explore through natural-language questions, draft analysis scripts, explanations of spatial results, and map narratives. The business value is faster discovery and communication, plus access for users who do not know GIS interfaces or query languages. Technical challenges include grounding responses in current, authoritative datasets; correctly handling coordinate reference systems, units, spatial joins, and scale; and preserving data lineage. A fluent response can still misstate a dataset’s coverage or produce a plausible but invalid workflow, so spatial outputs require direct verification by an analyst.

**Existing implementations:**
- [NASA Earth Copilot](https://www.earthdata.nasa.gov/news/feature-articles/earth-copilot): An experimental conversational interface for exploring NASA Earth science data, illustrating natural-language access rather than replacing geospatial analysis.
- [Esri ArcGIS AI assistants](https://www.esri.com/arcgis-blog/products/arcgis-online/announcements/arcgis-ai-assistants): Esri has described assistants that help users interact with ArcGIS content and workflows, with capabilities and availability varying by product and release.

### Software Development

Coding assistants generate or explain code, suggest completions, draft tests, and help developers navigate unfamiliar APIs. Their business value is reduced time on routine implementation and faster prototyping; a controlled GitHub study found faster completion of one programming task with Copilot, but that result does not guarantee gains across software projects. The main technical weaknesses are plausible but incorrect code, insecure dependencies or patterns, poor fit to a repository’s architecture, and uncertainty about licensing or provenance. Generated code still needs tests, code review, and security checks, particularly before it handles sensitive data or production systems.

**Existing implementations:**
- [GitHub Copilot](https://github.com/features/copilot): Provides code completion, chat, and other development assistance integrated with supported editors and GitHub workflows.
- [Amazon Q Developer](https://aws.amazon.com/q/developer/): Assists with coding, understanding, and working with software projects in AWS and supported development environments.
- [Gemini Code Assist](https://codeassist.google/): Offers generative coding assistance for development environments and Google Cloud workflows.

### Education

Conversational AI can provide practice, hints, explanations, and first drafts of learning materials, potentially making individualized support more available and helping educators with preparation. These tools can be useful for guided practice, but learning value depends on whether the system prompts students to reason rather than simply supplying answers. Technical and operational challenges include fabricated explanations, age-appropriate safeguards, student privacy, accessibility, uneven performance across languages and curricula, and measuring learning outcomes. Fluent feedback can be wrong or mismatched to a learner’s level, so teachers need oversight and students need ways to check answers against trusted materials.

**Existing implementations:**
- [Khanmigo](https://www.khanacademy.org/khan-labs): Khan Academy’s tutor and teaching assistant is designed to guide learners through problems and support educator planning.
- [Google AI for Education](https://edu.google.com/ai/): Google provides generative AI tools and resources for education settings, subject to institution and account configurations.
- [ChatGPT for Education](https://openai.com/index/introducing-chatgpt-edu/): OpenAI describes an institutional offering for universities with administrative controls and education-oriented access to its models.

### Healthcare Administration and Clinical Workflows

Clinical documentation assistants can draft visit notes from clinician–patient conversations, while other systems summarize records or retrieve information from approved sources. The business value is the possibility of reducing documentation burden and improving access to relevant information, allowing clinicians to spend more time on care when the workflow is effective. The challenges are substantial: speech recognition can miss names, medications, accents, or negation; generated notes can introduce unsupported details; and deployment must address patient consent, protected health information, clinical-system integration, and auditability. These systems are documentation aids, not autonomous clinicians, and a qualified professional must review and approve clinical records.

**Existing implementations:**
- [Microsoft Dragon Copilot](https://www.microsoft.com/en-us/health-solutions/clinical-workflow/dragon-copilot): Microsoft’s clinical workflow assistant combines ambient documentation and related clinical productivity capabilities for clinician review.
- [Abridge](https://www.abridge.com/): Generates clinical documentation from patient-clinician conversations and integrates with healthcare workflows.
- [Nabla](https://www.nabla.com/): Offers an AI assistant for clinical documentation and related administrative tasks.

### Drug Discovery and Life Sciences

Generative models can propose molecular structures or candidate proteins and help researchers prioritize which candidates to synthesize and test. The potential business value is a broader search space and more efficient early-stage experimentation, although the cost and duration of laboratory and clinical validation remain. Technical weak points include limited or biased training data, difficulty predicting whether a generated molecule can be synthesized or will behave safely in humans, and the gap between computational promise and clinical benefit. An AI-generated candidate is a hypothesis, not a medicine: experiments, regulatory review, and clinical trials are required to establish safety and efficacy.

**Existing implementations:**
- [Insilico Medicine Pharma.AI](https://insilico.com/pharmaai): A suite of AI-enabled drug discovery tools; a published case study describes a generative-AI-discovered TNIK inhibitor for idiopathic pulmonary fibrosis that advanced to clinical testing.
- [Published TNIK inhibitor study](https://doi.org/10.1038/s41587-024-02143-0): Reports the discovery and preclinical development of the candidate, while clinical testing remains necessary to establish patient outcomes.

### Media, Design, and Marketing

Image, text, audio, and video generators let creative teams rapidly explore concepts, produce variations, and adapt content for different formats. The business value is faster ideation and lower effort for some production tasks, not automatic replacement of creative direction or review. Technical and legal challenges include inconsistent brand details, inaccurate depictions, limited control over fine details, uncertain provenance, and possible resemblance to protected works or individuals. Outputs may also be generic or unsuitable for a campaign’s audience; organizations need review for factual accuracy, rights, consent, brand quality, and disclosure requirements.

**Existing implementations:**
- [Adobe Firefly](https://www.adobe.com/products/firefly.html): Provides generative image and design capabilities across Adobe creative products, with Adobe publishing information about its training and commercial-use approach.
- [Canva Magic Studio](https://www.canva.com/magic/): Brings generative text, image, and design tools into Canva’s visual content workflow.
- [OpenAI Sora](https://openai.com/sora/): Generates video from prompts and other inputs, supporting rapid visual prototyping while requiring review of fidelity, rights, and suitability.

### Enterprise Knowledge Work

RAG-based assistants can search internal documents and draft answers with supporting references, helping employees find procedures, product information, or institutional knowledge. The business value is faster information discovery and more consistent access to approved material, especially across large document collections. Technical challenges include indexing and updating sources, honoring access permissions, citing evidence, and integrating with existing identity and document systems. A model may still misread a document, combine incompatible sources, or invent an answer when retrieval fails; citations must be checked, sensitive records protected, and consequential advice kept under human control.

**Existing implementations:**
- [Morgan Stanley and OpenAI](https://openai.com/index/morgan-stanley/): Morgan Stanley describes an internal GPT-4 assistant that helps financial advisers search and summarize its approved knowledge base.
- [Glean](https://www.glean.com/): Provides enterprise search and AI assistance over connected workplace applications, with permissions and source context central to its offering.
- [Microsoft 365 Copilot](https://www.microsoft.com/en-us/microsoft-365/copilot): Adds generative assistance across Microsoft 365 applications and organizational content subject to tenant permissions and configuration.

## Benefits

- **Faster first drafts:** Drafting, summarization, code suggestions, and routine transformations can take less time, although review remains necessary.
- **More accessible interfaces:** Natural-language interaction can help people who do not know a specialized query language, programming language, or GIS interface get started.
- **Support for exploration:** Generating alternatives can help teams brainstorm, prototype, and compare possible approaches.
- **Scale across information sources:** When connected carefully to approved documents or data, a model can help users navigate large collections and synthesize relevant material.
- **Potentially broader participation:** Better interfaces may let more people engage with technical information, provided accessibility, language coverage, and representation are addressed.

These are potential or task-specific benefits, not guaranteed productivity or quality improvements. Outcomes depend on the task, model, data, user expertise, and review process.

## Challenges and Risks

- **Incorrect or fabricated output:** Language models can produce fluent statements, citations, code, or explanations that are wrong. Generated GIS workflows can be syntactically valid but spatially inappropriate.
- **Bias and uneven performance:** Training data may underrepresent languages, communities, regions, or population groups. In GIS, uneven data quality and geographic coverage can amplify these issues.
- **Privacy and confidentiality:** Prompts or connected data may contain personal, health, business, or sensitive location information. Teams need clear rules about data handling, retention, access, and approved services.
- **Copyright and provenance:** Generated material may raise questions about training data, attribution, ownership, and resemblance to existing work. Organizations should review tool terms and applicable law.
- **Security and misuse:** Prompt injection, unsafe generated code, and unauthorized access through connected tools can create risks. Tool permissions should be limited, outputs reviewed, and sensitive actions gated.
- **Reproducibility and changing behavior:** Model updates, prompt differences, and changing source data can produce different answers. High-impact workflows need versioning, logs, and repeatable validation.
- **Cost, infrastructure, and environmental impact:** Inference and deployment require compute, energy, and operational support. Small or conventional models may be a better fit for some jobs.
- **Overreliance and accountability:** Users may accept plausible responses without checking them. Organizations must define who approves outputs and who is accountable for decisions.
- **GIS-specific uncertainty:** Spatial data can be incomplete, outdated, misaligned, or measured at incompatible scales. A generated map narrative cannot fix flawed source data, and synthetic locations should not be mistaken for observations.

## Practical Guidelines for Responsible Use

1. Match the tool to the task. Use deterministic GIS operations or validated statistical models for computations that require exact, repeatable results; use GenAI where generation or flexible interaction adds value.
2. Ground answers in trusted sources. Connect assistants only to appropriate, current datasets or documents, and make source references visible to users.
3. Keep a human in the loop. Require qualified review before generated content is published or used for consequential decisions.
4. Test with representative cases. Evaluate factuality, spatial correctness, bias, privacy leakage, accessibility, and failure handling across the regions and users affected.
5. Protect data and control actions. Minimize sensitive inputs, apply least-privilege access, and require confirmation before an assistant edits data, runs code, or triggers external actions.
6. Document limitations. Record the model and data sources, known failure modes, review responsibilities, and procedures for correcting errors.

## Conclusion

Generative AI is being applied to software, education, healthcare workflows, scientific research, creative production, enterprise search, and geospatial data exploration. Its strongest practical role is often to help people find, draft, transform, or explain information—not to make unreviewed decisions. For GIS, conversational access to Earth science data and assistance with analysis workflows are promising, but geographic accuracy depends on reliable source data, correct spatial methods, and expert validation. Responsible adoption means measuring benefits in the intended workflow and treating verification, privacy, and accountability as core requirements.

## Selected References

1. NASA, “NASA Earth Copilot,” NASA Earth Science Data Systems. https://www.earthdata.nasa.gov/news/feature-articles/earth-copilot
2. Esri, “ArcGIS AI Assistants,” ArcGIS Blog. https://www.esri.com/arcgis-blog/products/arcgis-online/announcements/arcgis-ai-assistants
3. GitHub, “Research: quantifying GitHub Copilot’s impact on developer productivity and happiness,” 2022. https://github.blog/news-insights/research/research-quantifying-github-copilots-impact-on-developer-productivity-and-happiness/
4. Khan Academy, “Khanmigo,” product information. https://www.khanacademy.org/khan-labs
5. Microsoft, “Nuance DAX Copilot,” product information. https://www.microsoft.com/en-us/health-solutions/clinical-workflow/dragon-copilot
6. Ren, F. et al., “A generative AI-discovered TNIK inhibitor for idiopathic pulmonary fibrosis,” *Nature Biotechnology* (2024). https://doi.org/10.1038/s41587-024-02143-0
7. Adobe, “Adobe Firefly,” product information. https://www.adobe.com/products/firefly.html
8. OpenAI, “Morgan Stanley,” customer story. https://openai.com/index/morgan-stanley/
9. National Institute of Standards and Technology, *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile* (NIST AI 600-1, 2024). https://doi.org/10.6028/NIST.AI.600-1
10. UNESCO, *Guidance for Generative AI in Education and Research* (2023). https://unesdoc.unesco.org/ark:/48223/pf0000386693
