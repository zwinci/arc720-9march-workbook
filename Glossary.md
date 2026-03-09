1. Project and governance terms

These explain how the project is organized and controlled.
	•	Project Sponsor – business owner funding or backing the initiative
	•	Product Owner / Business Owner – person defining business needs and priorities
	•	Solution Architect – overall architecture owner
	•	Integration Architect – owner of integration design and patterns
	•	Technical Lead – lead developer for implementation details
	•	Steering Committee – governance body for major decisions
	•	Scope – what is included in the project
	•	Out of Scope – what is explicitly excluded
	•	Assumption – condition considered true for planning/design purposes
	•	Constraint – limitation affecting design or delivery
	•	Dependency – external item required for progress
	•	Risk – uncertainty with possible project impact
	•	Issue – current problem requiring action
	•	Decision Log – record of key architectural/business decisions
	•	RACI – roles and responsibilities model

2. Business and process terms

These align the integration with business meaning.
	•	Business Process – end-to-end operational flow
	•	Use Case – scenario describing how a business need is fulfilled
	•	Capability – business function supported by systems
	•	Business Event – occurrence that triggers processing
	•	Customer / Account / Order / Product / Invoice – core business entities
	•	Source System – system where data originates
	•	Target System – system receiving data
	•	System of Record – authoritative source for a data object
	•	Golden Record – most trusted consolidated version of data
	•	Master Data – shared core business data
	•	Reference Data – controlled lists such as countries, statuses, codes
	•	Transactional Data – operational data created during business execution
	•	Business Rule – rule governing validation or processing
	•	Exception – business or technical condition outside normal flow

3. Integration architecture terms

This is the heart of a MuleSoft glossary.
	•	Integration – exchange or orchestration of data between systems
	•	API-led Connectivity – MuleSoft approach using layered APIs
	•	System API – API exposing core systems with minimal business logic
	•	Process API – API orchestrating, transforming, or combining data
	•	Experience API – API tailored to a channel or consumer
	•	Application Network – connected reusable API ecosystem
	•	Integration Pattern – repeatable approach such as request-reply, pub/sub, batch
	•	Canonical Model – standard shared data model used across integrations
	•	Point-to-Point Integration – direct connection between two systems
	•	Orchestration – coordination of multiple calls/services into one flow
	•	Choreography – event-driven cooperation without central controller
	•	Synchronous Integration – caller waits for immediate response
	•	Asynchronous Integration – processing continues without immediate full response
	•	Real-time Integration – near-immediate processing
	•	Near Real-time – small acceptable delay
	•	Batch Integration – scheduled bulk processing
	•	Event-driven Integration – processing triggered by events/messages
	•	Pub/Sub – publisher sends events, subscribers consume them independently
	•	Polling – periodic check for new data/events
	•	Webhook – outbound callback triggered by an event
	•	Message Queue – asynchronous message buffer
	•	Topic – channel for publish/subscribe messages
	•	Dead Letter Queue (DLQ) – location for failed/unprocessable messages
	•	Replay / Redelivery – retrying message consumption
	•	Idempotency – repeated request produces same result without duplicates
	•	Correlation ID – identifier used for tracing across systems
	•	Sequence / Ordering – required message execution order
	•	Aggregation – combining data from multiple sources
	•	Routing – directing messages to the correct destination
	•	Transformation – converting data structure or format
	•	Enrichment – adding extra data to a payload
	•	Validation – checking structure, rules, or mandatory fields
	•	Mapping – correspondence between source and target fields
	•	Contract – expected interface behavior and payload structure

4. MuleSoft-specific platform terms

These are the core Mule concepts almost every project should define.
	•	Mule Application – deployable Mule runtime package
	•	Mule Runtime / Mule Runtime Engine – engine executing Mule applications
	•	Flow – main processing sequence in Mule
	•	Subflow – reusable internal flow
	•	Private Flow – internally callable flow
	•	Connector – component for connecting to external systems
	•	Listener – component receiving inbound requests/messages
	•	Processor – step that performs an operation in a flow
	•	Event – runtime object holding message and variables
	•	Message – Mule event content
	•	Payload – main business data in a Mule message
	•	Attributes – metadata associated with message/payload
	•	Variables – temporary context data inside a flow
	•	Properties – configuration values
	•	DataWeave – MuleSoft language for transformation
	•	Transform Message – Mule component using DataWeave
	•	Error Handler – flow logic for error processing
	•	Try Scope – scope for localized error handling
	•	Batch Job – Mule construct for bulk processing
	•	Scheduler – timed trigger for execution
	•	Object Store – persistence for state, watermark, idempotency, etc.
	•	Secure Properties – encrypted or protected config values
	•	Domain Project – shared resources/config for multiple Mule apps
	•	Reusable Asset – shared component/template/specification
	•	APIKit – framework for implementing APIs from specs
	•	RAML / OAS – API contract/specification formats
	•	Exchange – Anypoint repository for reusable assets
	•	API Manager – policy and lifecycle management for APIs
	•	Runtime Manager – deployment and runtime administration
	•	Anypoint Platform – overall MuleSoft platform
	•	CloudHub / CloudHub 2.0 / Runtime Fabric / On-Prem – deployment models
	•	VPC / Load Balancer / DLB – network deployment terms where applicable
	•	Business Group – Anypoint organizational unit
	•	Environment – dev, test, UAT, prod, etc.

5. API design and contract terms

Important for consistent API understanding.
	•	API Consumer – application or user calling the API
	•	API Provider – system/service exposing the API
	•	Endpoint – callable API path
	•	Resource – business object exposed by an API
	•	Method – GET, POST, PUT, PATCH, DELETE, etc.
	•	Request – inbound API call
	•	Response – API output
	•	Header – metadata sent with request/response
	•	Query Parameter – request filter/input in URL
	•	Path Parameter – variable part of endpoint path
	•	Body / Payload – content of request or response
	•	Schema – structure definition of payload
	•	Example – sample request/response
	•	Status Code – HTTP result indicator
	•	Pagination – split large result sets into pages
	•	Filtering – limit results by criteria
	•	Sorting – order result set
	•	Versioning – API version management
	•	Backward Compatibility – change that does not break consumers
	•	Breaking Change – change requiring consumer adjustment
	•	Consumer Contract – agreed API behavior and structure
	•	SLA – service level expectation
	•	Rate Limit / Throttling – control of consumer request volume
	•	Policy – runtime enforcement rule such as auth, rate limiting, CORS

6. Data and interface terms

Usually needed in every integration project.
	•	Interface – defined connection between two systems
	•	Inbound Interface – data/service entering Mule
	•	Outbound Interface – data/service sent from Mule
	•	Source-to-Target Mapping – mapping definition between systems
	•	Field Mapping – attribute-level transformation rule
	•	Mandatory Field – field required for processing
	•	Optional Field – field not always required
	•	Default Value – value used when source is missing
	•	Lookup / Crosswalk – translation between system codes/IDs
	•	Code Conversion – conversion of enumerations or statuses
	•	Data Quality – fitness of data for intended use
	•	Duplicate Record – same business entity appearing more than once
	•	Null Handling – rules for absent values
	•	Data Type – string, number, boolean, date, array, object, etc.
	•	Schema Validation – validation against structural contract
	•	Watermark – last processed timestamp/ID for incremental extraction
	•	Delta Load – process only changed records
	•	Full Load – process complete data set
	•	Upsert – insert or update based on key
	•	Natural Key – business-meaningful unique identifier
	•	Surrogate Key – system-generated identifier
	•	External ID – identifier from another system

7. Error handling and resilience terms

Very useful to define early.
	•	Error – technical or business failure
	•	Exception Handling – logic for processing failures
	•	Business Error – violation of business rule
	•	System Error – technical/runtime/infrastructure issue
	•	Recoverable Error – temporary issue that may succeed on retry
	•	Non-recoverable Error – permanent issue needing correction
	•	Retry – repeated attempt after failure
	•	Backoff – delay strategy between retries
	•	Timeout – allowed response duration before failure
	•	Circuit Breaker – protection against repeated failing dependency calls
	•	Fallback – alternative path when primary call fails
	•	Compensation – action to undo or offset a prior step
	•	Poison Message – message that repeatedly fails processing
	•	DLQ – queue for failed messages
	•	Alert – generated notification for support/action
	•	Incident – operational disruption requiring support
	•	Root Cause – underlying reason for failure

8. Security and compliance terms

These should always be in the glossary.
	•	Authentication – verifying identity
	•	Authorization – granting permissions
	•	Client ID / Client Secret – API consumer credentials
	•	OAuth 2.0 – delegated auth protocol
	•	JWT – token format carrying claims
	•	Basic Auth – username/password auth method
	•	Mutual TLS (mTLS) – certificate-based two-way trust
	•	TLS / HTTPS – transport encryption
	•	Encryption at Rest – stored data encryption
	•	Encryption in Transit – data transfer encryption
	•	Secret – protected credential/configuration item
	•	Certificate – digital trust artifact
	•	Key Rotation – periodic replacement of secrets/keys
	•	PII / Personal Data – personally identifiable data
	•	Sensitive Data – data needing restricted handling
	•	Data Masking – hiding sensitive values in logs or outputs
	•	Least Privilege – minimal required access rights
	•	Audit Trail – record of actions/events
	•	Compliance – adherence to internal or regulatory rules
	•	GDPR – data protection framework relevant in EU contexts

9. DevOps, environments, and release terms

Very common in enterprise MuleSoft delivery.
	•	Development / Test / UAT / Production – lifecycle environments
	•	Deployment – release of application into environment
	•	CI/CD – automated build, test, release pipeline
	•	Build Artifact – packaged deployable output
	•	Pipeline – automated deployment/test flow
	•	Promotion – moving release between environments
	•	Rollback – return to previous stable version
	•	Configuration Management – control of environment-specific settings
	•	Infrastructure as Code – scripted environment provisioning
	•	Release – packaged set of changes
	•	Hotfix – urgent production correction
	•	Downtime – planned or unplanned service unavailability
	•	Blue/Green Deployment – alternate deployment strategy
	•	Canary Release – limited exposure release strategy

10. Testing and quality terms

Should be present even in a default glossary.
	•	Unit Test – test of isolated logic/component
	•	MUnit – MuleSoft testing framework
	•	Integration Test – test with real or simulated dependencies
	•	System Test – end-to-end validation of integrated behavior
	•	Regression Test – confirms existing behavior still works
	•	Performance Test – measures speed, throughput, stability
	•	Load Test – checks expected volume handling
	•	Stress Test – checks behavior beyond normal volume
	•	Test Data – prepared input data for validation
	•	Mock / Stub – simulated dependency
	•	Acceptance Criteria – conditions for business acceptance
	•	Defect / Bug – deviation from expected behavior
	•	Quality Gate – required quality checkpoint before promotion

11. Monitoring and support terms

Essential for production support handover.
	•	Monitoring – active observation of application health
	•	Logging – recording runtime events
	•	Structured Log – machine-readable logging format
	•	Trace – end-to-end execution visibility
	•	Metrics – quantitative runtime measurements
	•	Dashboard – operational monitoring view
	•	Health Check – simple endpoint/process for runtime validation
	•	Availability – percentage of uptime
	•	Latency – response time
	•	Throughput – number of requests/messages processed in time
	•	Support Model – how incidents are handled
	•	L1 / L2 / L3 Support – operational support levels
	•	Runbook – operational instructions for common issues
	•	Knowledge Base – documented support and technical guidance

12. Non-functional requirement terms

These are usually expected in enterprise integration projects.
	•	NFR – non-functional requirement
	•	Availability – required uptime target
	•	Scalability – ability to handle increased load
	•	Performance – speed and responsiveness
	•	Resilience – ability to recover from disruption
	•	Maintainability – ease of support and change
	•	Observability – ability to understand system state from telemetry
	•	Recoverability – ability to restore service/data
	•	RTO – recovery time objective
	•	RPO – recovery point objective
	•	Capacity – supported transaction/message volume
