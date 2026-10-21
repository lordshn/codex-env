# Workplane — investor pitch deck

**Working name:** Workplane (name and trademark availability not checked).<br>
**Version:** concept / pre-seed discussion draft, October 21, 2026.<br>
**Audience assumption:** early-stage investors; also suitable for a design-partner discussion after removing financing slides.<br>
**Format:** 18 core slides + 3 appendix slides, intended for 16:9.<br>
**Product status:** discovery and research. Proposed capabilities are not implemented or validated customer outcomes. No customers, revenue, team credentials, partnerships or proprietary technology are claimed.<br>
**Narrative:** help a company publish an approved AI work environment and operate it with enforceable boundaries, useful evidence and measurable business outcomes. The product is a coherent application; backing integrations are implementation choices, not the customer proposition.

---

## 01 — Workplane

### Give every employee an approved way to work with AI.

A company control application for AI coding and agent workflows.

**One place to configure access, publish environments, govern supported runs and measure outcomes.**

Local models. External providers. Company-defined boundaries.

*Concept-stage investor discussion • October 2026 • Working name*

**Visual direction:** oversized headline; one concise product-definition block; three named domains—Environment / Intelligence / Control. No fictitious product screenshot.

**Presenter narrative:** Companies want employees to benefit from better AI tools without asking every employee to assemble the company's operating controls. Workplane proposes a supported path from company policy to real employee work.

---

## 02 — A license does not create a governed workflow

### Every new AI tool creates company decisions.

- **Data:** which code, context and memory can leave the company?
- **Authority:** which tools, credentials and actions can an agent use?
- **Economics:** who owns a run's spending, review effort and outcome?

Today, those decisions can be scattered across clients, gateways, workspaces and team conventions.

**The business problem: expanding AI use without a consistent operating model.**

*Problem framing; prevalence and willingness to pay remain to be validated.*

**Visual direction:** three equal panels, each connecting a company question to its operational consequence. Avoid a generic alarming breach image.

**Presenter narrative:** The gap is broader than buying model access. A company must know which path employees can use, what happens when a policy blocks work, and how it can stop or investigate a run.

---

## 03 — Agents make the operating model urgent

### AI now changes files, calls tools and executes commands.

**Permission boundaries are real engineering work.**<br>
Microsoft disclosed and patched agent approval and MCP permission vulnerabilities. [R1, R2]

**Faster output still requires verification.**<br>
Google engineers describe review, checking and integration overhead alongside AI benefits. [R3]

**Large-scale adoption is a program.**<br>
Accenture describes a pilot, controlled comparison and broader rollout on a managed development platform. [R4]

**The opportunity: make governed adoption repeatable.**

*Vulnerabilities are not evidence of exploitation. Research and customer-story findings have different evidentiary limits.*

**Visual direction:** three editorial evidence statements with company names in text, short citations and a single closing thesis.

**Presenter narrative:** These are signals of operating requirements, not proof our product has demand. The change from suggestions to actions increases the need for explicit authority, while productivity research tells us to measure completed work rather than generation alone.

---

## 04 — Start with the platform team

### One team owns the employee path into AI work.

**First users**<br>
Platform engineers and developers using company-provided cloud development environments.

**Internal champion**<br>
Head of Platform / Developer Experience.

**Joint decision makers**<br>
Engineering leadership and security; budget ownership validated during discovery.

**Initial customer hypothesis**<br>
Organizations with 500–5,000 engineers, an existing identity provider and cloud/Kubernetes platform, multiple AI services and meaningful data restrictions.

**First deployment: one engineering group, one supported workflow.**

*Customer profile and buying process are hypotheses.*

**Visual direction:** employee → platform champion → engineering/security buyer, shown as labeled columns rather than an org chart.

**Presenter narrative:** This audience already operates workspaces, identity and engineering tooling. We start where a supported employee workflow and a company control boundary can be tested together. We are not claiming that all companies need our preferred infrastructure.

---

## 05 — The core product: an approved AI work profile

### Configure once. Publish to the right employees.

An approved profile brings together:

- **Environment:** development tools, runtime and network boundaries.
- **Intelligence:** permitted models, memory sources and reusable skills.
- **Authority:** identity, tools/MCP, scoped access and approval rules.
- **Operations:** security workflow, resource limits and evidence settings.

**Employees launch a supported environment. The company can explain its effective configuration.**

*Proposed product experience; supported integrations are qualified individually.*

**Visual direction:** one large “AI work profile” panel with four clearly named sections and a Publish action. Label this as a product concept, not a working interface.

**Presenter narrative:** This is our most valuable capability: a company distributes an understandable, governed combination of AI capabilities instead of distributing raw integration settings and privileged keys. An administrator should be able to answer what applies to a given employee and task.

---

## 06 — From company policy to useful employee work

### A single launch-to-revocation experience.

**1. Configure**<br>
Connect identity, approved services and an environment template.

**2. Publish**<br>
Assign a reviewed work profile to a group or project.

**3. Work**<br>
Employee starts the environment; supported model and tool operations follow policy.

**4. Operate**<br>
Review outcomes and cost, resolve exceptions, revoke access or stop a run.

**Illustrative task:** investigate a service issue and propose a reviewed code change, without receiving production write access.

*Concept workflow, not implemented functionality.*

**Visual direction:** four sequential numbered stages; employee action and company control visibly paired.

**Presenter narrative:** The business outcome is getting to approved, useful work quickly and keeping that work operable over time. Offboarding and incident containment belong in the same story as onboarding.

---

## 07 — Control data before dispatch; bound actions before execution

### Security is a workflow with explicit enforcement points.

**Before a model request**<br>
Check eligible context and destination; apply configured secret/sensitive-data checks; allow, redact, route, block or request review.

**Before a tool action**<br>
Check identity, resource scope, arguments and approval; execute only within the permitted runtime and network boundary.

**After the decision**<br>
Record minimized evidence tied to the policy, run and outcome.

**No universal detection promise. No silent local-to-external fallback.**

*Scope: supported, instrumented paths. Controls need adversarial testing; ungoverned clients require separate restrictions. A scanner is itself a data recipient.*

**Visual direction:** two parallel, clearly labeled flows—model dispatch and tool action—feeding one evidence block. Use text and simple boxes; no invented dashboard metrics.

**Presenter narrative:** A gateway alone cannot bound every shell command or credential read. Our product promise must name the exact supported paths and use independent network, runtime and authorization controls. Failed or uncertain checks need an explicit company-defined response.

---

## 08 — Local, cloud or hybrid: company policy decides

### Choose the service without losing the boundary.

**Internal-only work**<br>
Use qualified internal inference and required internal dependencies.

**Approved external work**<br>
Send eligible data only to approved providers under configured rules.

**Hybrid work**<br>
Select permitted services by use case, data class and capability; failover stays within the same policy boundary.

**The same choice applies to memory, retrieval, inspection and decision services—not only the main LLM.**

*Configuration requires supported adapters and qualification. Hosting location alone is not a security guarantee.*

**Visual direction:** three policy examples with the shared company policy band above them. Show internal and external as locations, not “safe/unsafe” labels.

**Presenter narrative:** We should not force one hosting ideology. The company owns its permitted destinations and service choices. Moving inspection or embeddings outside the company is also external processing and must be visible.

---

## 09 — Reusable context needs ownership

### Make memory, skills and tools company-managed capabilities.

**Memory and knowledge**<br>
Define source access, scope, provenance, retention and deletion behavior.

**Skills and MCP tools**<br>
Publish reviewed versions with scoped permissions and clear owners.

**Specialist decision models — expansion**<br>
Configure evaluated classification, routing or escalation functions using permitted local or external services.

**Model judgments can inform workflow; they cannot grant authority.**

*Memory backends have different semantics. Broad interchangeability and decision-model functions are later qualification work, not launch promises.*

**Visual direction:** three editorial blocks around the words “Owner / Version / Scope / Lifecycle.” Keep specialist models subordinate to the launch proposition.

**Presenter narrative:** The vision goes beyond model routing, but breadth can sink the first release. We qualify one context path first. Jev/Clef-style functions can later help select relevant context or escalate uncertainty, within hard company constraints.

---

## 10 — Prove value with the complete task

### Measure useful work, operating effort and total cost together.

| Outcome | Pilot measure |
|---|---|
| Faster access | Time from approval to first useful employee task |
| Lower platform burden | Setup, integration and exception-handling hours |
| Controlled spending | Full cost per verified outcome, with owner attribution |
| Reliable work | Review effort, rework, defects and delivery stability |

**Pass the pilot only if employee value improves without unacceptable security, quality or operating regressions.**

*Targets set with the design partner against a local baseline. No productivity uplift or cost saving is claimed.*

**Visual direction:** four large outcome labels with a compact measurement row beneath each; no fabricated before/after bars.

**Presenter narrative:** Token price and coding speed are incomplete. We include inference, compute, tools, operation and review effort. Google/DORA's work supports this broader measurement approach [R3, R5].

---

## 11 — A focused entry market; a transparent sizing model

### Begin where AI adoption meets platform and security ownership.

**Entry segment**<br>
Engineering organizations with multiple AI tools, company-managed environments and restrictions on data or actions.

**Illustrative account value**<br>
$78,000 annual software contract at 200 active users under the proposed pricing model.

**Bottom-up opportunity scenarios — unvalidated**

| Assumed eligible organizations | At $78k annual contract value |
|---|---|
| 5,000 | $390m annual software opportunity |
| 50,000 | $3.9bn annual software opportunity |

**First commercial milestone: 10 paid customers = $780k ARR at that contract value.**

*Arithmetic scenarios, not researched TAM/SAM, customer counts, forecast or contracted revenue. Validate account population, willingness to pay and attainable penetration before external fundraising use.*

**Visual direction:** account-value equation plus two clearly labeled scenario rows. Avoid a fabricated market-growth chart.

**Presenter narrative:** We do not yet have a validated market count. This slide makes the commercial thesis testable: identify eligible organizations, discover the actual budget and conversion path, then replace these scenarios with a sourced account model.

---

## 12 — Close competitors exist

### Win on a demonstrably better operating experience.

| Alternative | Documented center of gravity |
|---|---|
| Coder | Company development environments, agents and AI governance |
| Agyn | Company console for providers, agents, skills and execution |
| Preloop | Model/tool governance, policies, approvals and run control |
| OpenHands Enterprise | Enterprise software-agent execution and management |
| Internal assembly | Existing workspaces, gateway, identity and security tooling |

**Our differentiation hypothesis:** publish one effective work profile and carry its policy through context, execution, evidence and revocation—with less integration burden.

**Proof required:** run the same customer workflow against the strongest alternatives and measure setup effort, coverage and ongoing operations.

*Public documentation comparison; capabilities vary by edition. No claim that competitors lack these outcomes. Sources: R6–R9.*

**Visual direction:** neutral text comparison; emphasize the validation challenge rather than unsupported checkmarks.

**Presenter narrative:** This is not an uncontested category. A broad feature list is not a moat. The test is whether we make a particular company's approved employee workflow materially easier to provide and operate than a nearby product or internal assembly.

---

## 13 — Subscription software; customer-controlled services

### Charge for operating the company’s AI work platform.

**Proposed annual pricing hypothesis**<br>
$18,000 platform fee + $25 per monthly active employee per month.

**Example**<br>
200 active employees × $25 × 12 + $18,000 = **$78,000 ARR**.

**Customer pays separately**<br>
Model inference, infrastructure and third-party services; support scope and deployment options defined in contract.

**Proposed entry offer**<br>
$10,000, eight-week paid pilot; credit toward the first annual contract upon conversion.

*Illustrative USD pricing, not a quote. Validation needed: procurement fit, support cost, margin and willingness to pay. ARR excludes pilots and pass-through usage.*

**Visual direction:** large pricing equation, small cost-boundary panel. No invented gross-margin percentage.

**Presenter narrative:** Our revenue should align with the company operating value rather than rely on hidden token margins. A paid pilot tests whether the budget is real. A managed service or self-hosted support model needs separate cost validation.

---

## 14 — Land with a bounded workflow; expand with evidence

### Sell an adoption outcome before a platform-wide transformation.

**Recruit**<br>
Three design partners through platform-engineering and security relationships; introductions are a planned activity, not an existing pipeline.

**Pilot**<br>
One engineering group, 20–50 users, one environment/agent combination and a defined set of tools and data flows.

**Convert**<br>
Annual agreement after agreed value, security and operating criteria pass.

**Expand**<br>
More groups, qualified capabilities and governed workloads within the same company.

**Primary sales evidence:** time to approved work, platform effort and cost per accepted outcome.

*Proposed go-to-market plan; no partner or customer commitment is claimed.*

**Visual direction:** four-stage motion with the pilot scope visually prominent.

**Presenter narrative:** We avoid asking a company to replace its entire development platform. The first sale is a concrete workflow, an accountable sponsor and a measurable acceptance decision. Sales-cycle length and acquisition economics remain unknown.

---

## 15 — Build a narrow product before a broad catalog

### Validate the core loop, then extend the capability surface.

**Months 0–3 — Design-partner proof**<br>
Confirm buyer and budget; prototype publishing and launching one work profile; establish baselines and threat model.

**Months 4–9 — Qualified pilot product**<br>
One environment/agent stack; OIDC; approved model connections; defined pre-egress checks; scoped tool access; attribution and revocation tests.

**Months 10–18 — Repeatable deployment**<br>
Harden reliability and upgrades; qualify a second model path; validate governed memory; improve administration and conversion economics.

**Later expansion:** broader adapters, decision functions and more employee workflows.

*Illustrative sequence dependent on staffing and technical discovery; not a committed release schedule. Production readiness requires documented acceptance testing, not a calendar date.*

**Visual direction:** three large milestone blocks with acceptance outcomes below; use a timeline, not a product architecture diagram.

**Presenter narrative:** The gateway, memory and environment engines remain choices to evaluate. This pitch does not commit to Che, LiteLLM, OmniRoute or a specific deployment architecture. The product owns the coherent experience and supported behavior.

---

## 16 — Turn integration work into a repeatable product

### The potential moat is earned through execution.

**Reusable operating knowledge**<br>
Qualified adapters, compatibility tests and safe configuration migrations.

**Trusted workflows**<br>
Evaluated policy behavior, revocation paths and customer-specific acceptance evidence.

**Embedded administration**<br>
Published profiles and lifecycle workflows that remain portable and understandable.

**Key risks to retire**<br>
Incumbent convergence, support-heavy integrations, imperfect inspection and uncertain willingness to pay.

*No proprietary dataset, patent, network effect or established defensibility is claimed. Customer content is not assumed available for training.*

**Visual direction:** three value-building columns over one concise risk strip.

**Presenter narrative:** Open-source components accelerate development, but do not by themselves make a defensible business. We would need a demonstrated advantage in reliability, operational effort and customer outcomes, while keeping configurations portable.

---

## 17 — Concept stage: the next proof is customer proof

### Research supports the problem. It does not establish product-market fit.

**Completed discovery inputs**<br>
Capability inventory; adjacent-product research; company adoption and governance evidence.

**Not yet established**<br>
Paying demand, deployment results, validated economics or product security.

**Founding capabilities required**<br>
Platform/runtime engineering; enterprise security and identity; developer-product design; technical enterprise sales.

**Team status**<br>
Founder names, credentials, current staffing and hiring commitments have not been provided.

*Replace with a factual team slide before investor circulation. No traction is implied by research activity.*

**Visual direction:** evidence-to-validation split with a short founding-capabilities band. Do not invent headshots or logos.

**Presenter narrative:** An investor needs to know who can execute this. We cannot invent those details. This draft makes the gap explicit and focuses the next stage on buyer interviews, willingness to pay and hands-on comparative trials.

---

## 18 — Fund the proof of a repeatable company rollout

### Proposed pre-seed ask: $2.0m for an 18-month validation program.

**Illustrative allocation**<br>
$1.4m product, engineering and security; $0.3m customer development; $0.3m infrastructure, legal and operating reserve.

**Success criteria to validate**

- Three completed design-partner pilots, with at least two annual conversions.
- Repeatable installation, profile publishing and employee onboarding.
- Tested authorization, data-flow coverage, revocation and recovery for the supported scope.
- Evidence of buyer value and sustainable deployment/support economics.

**Build the approved path into AI work.**

*Funding amount, runway, allocation and milestones are planning assumptions; founder budget, geography and hiring plan are unknown. No live raise or financing terms are asserted.*

**Visual direction:** large ask, three allocation amounts, four measurable proof points. Treat the allocation as labeled numbers rather than a chart unless a real planning chart is requested.

**Presenter narrative:** The purpose of the round is to retire product, security, deployment and commercial risks. This is an example financing narrative that must be reconciled with the founders' actual plan before any investor solicitation.

---

## 19 — Appendix: what the first release must prove

### Company controls need tests, not only settings.

| Area | Proposed acceptance evidence |
|---|---|
| Identity and action scope | Denied cross-user/resource access; bounded and expiring approvals |
| Data paths | Defined scanner coverage, bypass tests and failure behavior before dispatch |
| Context lifecycle | Source access enforced; retention and derived-data deletion verified |
| Cost and reliability | Scoped run limits, retry caps, cancellation and attribution tested |
| Operations | Revocation, patching, recovery and privacy-limited investigation demonstrated |

**Specialist models remain advisory to policy. Uncertain results cannot override a hard deny or supply approval.**

*Acceptance categories for discovery; architecture and test thresholds not yet agreed.*

**Visual direction:** compact acceptance matrix, visually distinct from marketing capability claims.

**Presenter narrative:** The word “governed” must correspond to documented, tested behavior. We cannot promise total leakage prevention or rely on model confidence as an authorization decision.

---

## 20 — Appendix: evidence behind the timing and problem

### Primary sources; no invented breach or savings claims.

**R1 — Microsoft:** agent custom-hook approval vulnerability and fix.<br>
https://github.com/microsoft/vscode/security/advisories/GHSA-fq62-m6f5-c7h9

**R2 — Microsoft:** shared MCP sandbox permission grants and fix.<br>
https://github.com/microsoft/vscode/security/advisories/GHSA-qghm-w43w-vx8v

**R3 — Google / DORA:** qualitative analysis of 1,110 Google engineer responses; verification and integration themes; SEQ measurement.<br>
https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/insights/balancing-ai-tensions/index.md

**R4 — GitHub / Accenture:** pilot, controlled comparison and managed development-platform choices; vendor/customer story.<br>
https://github.com/customer-stories/accenture

**R5 — DORA:** AI ROI framework; planning model, not realized company savings.<br>
https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/ai/roi/report/index.md

*Sources reviewed October 21, 2026. R1–R2 do not establish exploitation; R3 is qualitative self-report; R4 does not provide universal productivity effect sizes; R5 is a model.*

**Visual direction:** two-column bibliography with short clickable labels in the final slides; full URLs remain in this companion source document.

---

## 21 — Appendix: competition and assumptions

### The differentiation and business model remain hypotheses.

**R6 — Coder:** released AI governance documentation; commercial/edition boundaries apply.<br>
https://github.com/coder/coder/blob/v2.38.1/docs/ai-coder/ai-governance.md

**R7 — Agyn:** company management console and adjacent configuration domains.<br>
https://github.com/agynio/platform/blob/6a778d39828aaf096dbe2b7f2ea676a48957404b/docs/administer/console-overview.md

**R8 — Preloop:** product scope and edition matrix.<br>
https://github.com/preloop/preloop/blob/1292a7bf59ff7963f74adcb4989a4339e27512fc/README.md

**R9 — OpenHands:** enterprise versus open-source scope.<br>
https://github.com/OpenHands/docs/blob/2ae24ad19e64d69ffc54e09e68af3de203cfffa0/enterprise/enterprise-vs-oss.mdx

**Explicit assumptions:** investor audience; working brand; target customer; $78k example annual contract; unvalidated opportunity scenarios; pilot offer; rollout timing; founding-team needs; $2m funding narrative.

**Before external circulation:** confirm team and company identity; validate buyer and market counts; agree pricing and financing; qualify technical promises; refresh competitor sources.

*The deck is a proposed business narrative, not an approved architecture, financial forecast or production-security representation.*

**Visual direction:** concise bibliography above a clearly marked assumption band.
