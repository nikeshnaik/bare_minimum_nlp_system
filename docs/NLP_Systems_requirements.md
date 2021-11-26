# NLP Systems

Last Edited: November 26, 2021 3:39 PM

### Requirements:

1. Build an NLP system with a high-level design having Components NLP tasks. Each Task must be loosely coupled and can be replaced with a new one.
2. NLP system will be deployed as API or Conversational Interface or Search or Package.
3. Additional components could be added as necessary to the above.
4. Each component can have an API endpoint.
5. Component must be a separate NLP Task, can have a different tech stack than another task.
6. The whole NLP System must have a faster iteration possibility, each component can be removed or added or trained, or modified quicker using config.
7. Each NLP task can be solved based on heuristics or models.
8. NLP systems can be used in different domains like healthcare to retail based on changes in model embedding or heuristic rules
9. Fully Customizable / Low Complexity / High Latency / Ease of Maintenance
10. No need for what to do after the end of the NLP Pipeline as this NLP System can be used as a pre-stage before finding any information or business logic.

### Non Functional Requirements:

1. Low Latency
2. High Availability even if models are getting updated or go out of memory by defaulting to rule-based models.
3. Model Consistency is not expected as NLP models are known to be non-interpretable
4. System Consistency is also not expected.

### List of Components of NLP System Necessary for v1:

- Auto-correct is based on the domain where the NLP system is used and customizable for a customer.
- Preprocessing Steps
- Rule-based NER
- Rule-based Intent Classification

### List of Components of NLP System Necessary for v2

- Auto-Correct with Word Embeddings
- Preprocessing Steps
- ML model for NER, transfer learning only, using hugging face or 3rd party library like Spacy with Rule-based Filtering above it
- ML Model for Intent classification, transfer learning only, using hugging face or 3rd party library like spacy with Rule-based Filtering above it.

### List of Components of NLP System V3

- Literally use all NLP tasks available in the world. Final Destination.
- Language can also be added if needed.

 

### Deployment

- FastAPI + Dockerize each component and deploy with Swarm
- Each Model must have an endpoint with Swagger Integration