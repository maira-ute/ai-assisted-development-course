# Generative AI Vocabulary

A plain-language glossary for people designing, building, evaluating, or using generative AI applications. GIS-specific terms are included because this course focuses on geospatial applications.

## Core Concepts

- **Artificial intelligence (AI):** Computer systems performing tasks that usually need human judgment, such as recognizing patterns, generating text, or making predictions.
- **Artificial general intelligence (AGI):** A hypothetical AI with broad abilities comparable to a person across many different kinds of tasks; current GenAI tools are not AGI.
- **Foundation model:** A large model trained on broad data that can be adapted or prompted for many different tasks.
- **Generative AI (GenAI):** AI that creates new content, such as text, images, audio, video, code, or structured data.
- **Large language model (LLM):** A model trained on large amounts of text to understand and generate language; it can also work with code and other inputs.
- **Machine learning (ML):** A way to build computer systems that learn patterns from examples instead of relying only on hand-written rules.
- **Model:** The learned mathematical system that takes input and produces an output, such as a prediction or generated response.
- **Multimodal model:** A model that can work with more than one kind of information, such as text and images or audio and video.
- **Neural network:** A computer model made of connected mathematical operations that learns patterns from data.
- **Training:** The process of adjusting a model using data so it learns patterns and can perform a task.
- **Transformer:** A neural-network design used by many modern language models to process relationships among words and other parts of an input.

## Working With Models

- **API (application programming interface):** A defined way for one software application to request a service or data from another, such as sending a prompt to an AI model.
- **Context window:** The amount of text and other input a model can consider in one request, including the conversation and supplied documents.
- **Embedding:** A list of numbers that represents the meaning or features of text, images, or other data so a system can compare similar items.
- **Fine-tuning:** Further training a model on a narrower set of examples to make it better suited to a particular task or style.
- **Inference:** Using a trained model to produce an answer or other output.
- **Latency:** How long a user waits for a system to respond.
- **Model provider:** The organization that supplies or hosts a model.
- **Open-weight model:** A model whose learned weights are available for others to download or run, often subject to a license; this does not necessarily mean its training data or code are open.
- **Parameter:** A learned value inside a model; large models can have billions of these values.
- **Prompt:** The instructions, question, examples, and context provided to a model for a particular request.
- **Prompt engineering:** Designing and refining prompts to help a model produce more useful, consistent results.
- **Rate limit:** A restriction on how many requests or how much data an application can send to a service in a given time.
- **Temperature:** A setting that influences how varied or predictable a model’s generated output is; lower settings generally produce less variation.
- **Token:** A small unit of text processed by a language model; it may be a whole word, part of a word, or punctuation.
- **Throughput:** How much work a system can complete over a period of time, such as requests per second.
- **Tool calling:** A model’s ability to request an action from an external function or service, such as searching a database or running a calculation.

## Data, Search, and Grounding

- **Chunking:** Splitting a long document into smaller sections so a system can find and provide relevant parts to a model.
- **Data provenance:** Information about where data came from, how it was collected, and how it has been changed or used.
- **Grounding:** Connecting a model’s response to trusted information, data, or tool results instead of relying only on what it learned during training.
- **Hallucination:** A confident-sounding model response that is made up, unsupported, or incorrect.
- **Knowledge base:** A collection of documents or structured information that an application searches to answer questions.
- **Retrieval:** Finding relevant information from a collection in response to a query.
- **Retrieval-augmented generation (RAG):** A method that retrieves relevant information first, then gives it to a generative model to help produce an answer based on those sources.
- **Semantic search:** Searching by meaning rather than requiring an exact match of the words used in the query.
- **Vector database:** A database designed to store and search embeddings, often used to find text or other items with similar meaning.

## Application Design and Evaluation

- **AI agent:** An AI application that can plan or carry out steps using tools, such as searching, calculating, or updating a system; its permissions and actions should be limited and monitored.
- **Application workflow:** The sequence of steps that a user and software follow to complete a task.
- **Benchmark:** A defined test used to compare model or application performance on selected tasks.
- **Evaluation:** Testing whether an AI application is accurate, useful, safe, fast, and appropriate for its intended users and tasks.
- **Human-in-the-loop:** A workflow where a person reviews, approves, or corrects AI output before it is relied on or acted upon.
- **Guardrail:** A rule or technical control that limits unsafe or unsuitable inputs, outputs, or actions.
- **Observability:** The ability to inspect how an application behaves, including its inputs, outputs, errors, speed, and use of tools.
- **Proof of concept (PoC):** A small trial built to find out whether an idea is technically possible or useful before investing in a full product.
- **Prototype:** An early version of an application used to test a design or workflow; it may not be ready for real-world use.
- **Prompt template:** A reusable prompt structure with spaces for information that changes from one request to another.
- **System prompt:** Instructions that define the model’s role, boundaries, or response style within an application.
- **Test set:** A collection of examples used to check an AI system; it should reflect the real tasks and users the system will encounter.

## Safety, Privacy, and Governance

- **Access control:** Rules that determine which users or systems are allowed to see data or perform actions.
- **Bias:** A systematic pattern of unfair or uneven results, which can come from training data, system design, or how a tool is used.
- **Data minimization:** Collecting or sending only the information needed for a task.
- **Explainability:** How well people can understand why a system produced a result; a fluent explanation is not necessarily a faithful account of a model’s internal process.
- **Human oversight:** People’s responsibility to monitor and review a system, especially when errors could cause harm.
- **Model drift:** A decline or change in performance as real-world data, user needs, or conditions shift over time.
- **Personally identifiable information (PII):** Information that can identify a person, such as a name combined with contact or account details.
- **Privacy:** Protecting information about people from being collected, exposed, or used in ways they did not expect or permit.
- **Prompt injection:** An attempt to manipulate an AI system by placing instructions in user input or retrieved content that conflict with its intended rules.
- **Red teaming:** Deliberately testing a system with difficult or adversarial inputs to find weaknesses before or after release.
- **Responsible AI:** Designing and using AI with attention to safety, fairness, privacy, transparency, and accountability.
- **Security:** Protecting the system, its data, and its tools from unauthorized access, manipulation, or misuse.
- **Synthetic data:** Artificially generated data used in place of or alongside real data; it may still preserve sensitive patterns or fail to represent reality well.

## GIS and Geospatial Terms

- **Coordinate reference system (CRS):** The rules that define how locations on Earth are represented as coordinates on a map.
- **Earth observation:** Information about Earth collected by satellites, aircraft, drones, or other sensors.
- **Geocoding:** Converting a place description, such as a street address, into geographic coordinates.
- **Geospatial data:** Information linked to a location on Earth.
- **Geospatial workflow:** A sequence of operations that prepares, analyzes, or displays location-based data.
- **Map scale:** The relationship between distances on a map and the corresponding distances on the ground; the appropriate scale affects which patterns can be seen.
- **Raster data:** Geographic information stored as a grid of cells or pixels, such as a satellite image or elevation model.
- **Resolution:** The level of detail represented in data; for a raster image, it often refers to the ground area represented by each pixel.
- **Spatial analysis:** Using location and geographic relationships to answer questions, such as which homes are near a flood zone.
- **Spatial join:** Combining records based on where their features are located relative to one another.
- **Vector data:** Geographic features represented as points, lines, or shapes, such as wells, roads, or administrative boundaries.

## Common Distinctions

- **AI versus GenAI:** AI is the broad field; GenAI is the part that creates new content. A system that classifies land cover may use AI without being generative.
- **Fine-tuning versus RAG:** Fine-tuning changes a model through additional training; RAG supplies relevant information at answer time without changing the model’s learned weights.
- **Model versus application:** A model generates outputs; an application combines the model with prompts, data, software, user controls, and review processes to accomplish a task.
- **Prototype versus production system:** A prototype explores an idea; a production system is deployed for ongoing use with operational support, security, monitoring, and accountability.
- **Prediction versus generation:** Prediction estimates an outcome or label; generation creates new content. Some applications combine both.
- **SME (subject matter expert):** A person with deep knowledge of a specific field who can judge whether an AI-generated result makes sense in that field.
