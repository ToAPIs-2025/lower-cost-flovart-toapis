# Provider integration proposal

Experimental opt-in UserScript JSON provider proposal; preserve RunningHub release path and shared durable Workflow authority. Real independent API outputs tested; Browser Workflow, durable Artifact import and creative-host acceptance remain unverified.

Modules: `services/userScriptProviderAdapter.ts; registerUserScriptProvider; provider credential reference; shared task/artifact store`.

## Required acceptance

Query `/v1/pricing` with the actual generating Key and exact conditions before each intended paid request. Match model, auth, body, asynchronous task query and result paths explicitly. Persist the business/task identity before submission; reconcile unknown submissions instead of retrying POST. Retain pending, settled and refunded billing separately. Download and validate media before importing a durable asset. Keys, balances and raw task IDs remain private. Cancellation of local polling does not establish an upstream refund. Seedance Global is disabled.

Full application, UI and deployment checks remain pending; a contract replay does not establish them.

UserScript is a restricted JSON mapping, not arbitrary JavaScript. The definitions here are experimental references. Current source keeps the adapter task handle locally during execute; durable host reconciliation, preflight pricing and artifact import must be connected before enabling this route in production. RunningHub remains the release certification path; Resolve and other host integrations are not certified by this API example. Root LICENSE currently says MIT while CONTRIBUTING still mentions AGPL-3.0-only; clarify contribution terms before an upstream code PR.
