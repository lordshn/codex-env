# Why Companies Need an AI Coding and Agent Adoption Plan

## An evidence-based business case for governing employee AI use

**Prepared:** October 21, 2026  
**Audience:** executive leadership, engineering, security, platform engineering, finance and data owners  
**Purpose:** explain the business and operating risks of unmanaged AI adoption, and the decisions a company needs to make before expanding AI-assisted coding and agentic work.

## Executive summary

AI coding assistants and agents can help employees draft, investigate, learn, automate and deliver software. Their business value depends on the system around them: authorized data, reliable environments, suitable tools, review capacity, cost controls and accountable ownership. A company that purchases AI subscriptions without planning these boundaries can increase activity while losing visibility into its data, permissions, spending and software-delivery outcomes.

The change is especially important when AI progresses from suggesting text to executing commands, calling tools, using credentials and retaining memory. A mistaken answer can become an unauthorized action. A document or tool response can influence an agent. A cheap individual request can become an expensive multi-step run. An apparently faster coding task can create additional review, verification and production-integration work.

The evidence supports both opportunity and caution:

- **Accenture** describes a small pilot, a larger controlled comparison and phased Copilot rollout alongside centralized identity, administration and security tooling. This is an example of planned adoption, not a license-only deployment. [S1](https://github.com/customer-stories/accenture)
- **Google's researchers** analyzed 1,110 open-ended responses from Google engineers and identified benefits alongside verification, review and integration burdens. Google uses speed, ease and quality indicators rather than a single code-volume measure. [S2](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/insights/balancing-ai-tensions/index.md)
- **GitLab** publishes engineering practices covering human accountability, confidential-data handling, AI-assistance disclosure, deterministic checks and increasing autonomy only as the surrounding engineering system matures. [S3](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/946c9f1441d92caa142091e0678e7dbdac3d38c3/content/handbook/engineering/infrastructure-platforms/developer-experience/ai/_index.md) [S4](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/5f92de4547bca68f41f5ec784e621f097c1e8b38/content/handbook/engineering/workflow/ai-assisted-development.md)
- **Microsoft** disclosed concrete agent approval and MCP permission vulnerabilities and issued fixes. This demonstrates that agent governance includes maintaining software permission boundaries, not only writing acceptable-use instructions. These advisories do not establish exploitation or a corporate breach. [S5](https://github.com/microsoft/vscode/security/advisories/GHSA-fq62-m6f5-c7h9) [S6](https://github.com/microsoft/vscode/security/advisories/GHSA-qghm-w43w-vx8v)

The appropriate response is an adoption program with supported use cases, approved services, enforceable access and data rules, measured outcomes, staged autonomy and a clear incident/recovery path. It can use local models, cloud providers or both. Location alone does not establish safety, value or control.

**Executive recommendation:** fund a bounded, measurable adoption program and assign ownership for its operating controls. Expand access and autonomy when local evidence shows useful outcomes at an acceptable level of risk and total cost.

## 1. What changes when employees use AI agents

An employee's AI workflow may involve more than a model endpoint. It may assemble source code, instructions, conversation history, internal documents, retrieved memory, tool descriptions and tool results. It may then call additional models, run shell commands, access repositories or cloud services, and preserve results for later sessions.

This creates several questions that ordinary software procurement does not answer:

1. Which data and credentials can each part of the workflow access?
2. Which services receive that data, including telemetry, embeddings and safety checks?
3. What actions may the agent perform, for which employee and on which resources?
4. What remains under human review, and how is approval enforced?
5. What does a completed, verified task actually cost?
6. How are errors, access changes, incidents and retained information handled?

A model may behave correctly while its permissions are too broad. A security filter may work while another extension sends data through a different route. An agent may generate valid code that is expensive to review or unsafe to operate. A plan must cover the complete supported workflow.

## 2. What major companies' experience actually shows

The examples below have different evidentiary meanings. A **disclosed vulnerability** is not necessarily an exploited incident. A **published working practice** is not proof every team implements it. A **vendor/customer story** is not an independent audit. A **research result** must remain tied to its population and methods. None of the companies is presented as having adopted AI without any governance.

### 2.1 Accenture: evaluate adoption and build on a managed platform

**The challenge.** Large organizations need to determine whether AI assistance helps their developers and how to make adoption repeatable. Existing identity, repository administration and security work also consume time. In GitHub's customer story, an Accenture architecture leader describes the cost of building and managing their own tools as an organizational concern. [S1](https://github.com/customer-stories/accenture)

**What Accenture chose.** The story describes an initial 20-developer Copilot pilot, followed by an Accenture/Microsoft controlled comparison involving 450 Copilot users and 200 controls, then broader rollout. It also documents Microsoft Entra ID for repository access, IssueOps/GitHub Actions administration, and an Information Security mandate for GitHub Advanced Security. These platform controls are documented organizational choices; the story does not establish that all were introduced because of Copilot.

**What the evidence supports.** The story reports more successful builds and weekly pull requests, but does not provide effect sizes or uncertainty for those outcomes. It supports the value of phased evaluation and repeatable platform controls. It does not establish a universal productivity percentage or a quantified company-wide AI cost saving.

**Business lesson.** Treat AI adoption as an evaluated change to a managed development system. Decide who receives access, which controls apply and how results will be measured before scaling.

### 2.2 Google: verification and review are part of productivity

**The challenge.** Faster drafting can move effort into checking, reviewing and integrating the output. A DORA analysis published March 10, 2026 examined 1,110 open-ended responses from Google software engineers collected in Q3 2025. Engineers described benefits in drafting, boilerplate, learning and synthesis, alongside verification overhead, reviewer burden and a gap between prototype generation and production-ready integration. [S2](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/insights/balancing-ai-tensions/index.md)

**What Google measures.** The authors state that Google uses **speed, ease and quality (SEQ)** as developer-productivity indicators. Their recommendations include holistic measurement, earlier feedback, smaller reviewable changes and attention to integration and tool-selection friction. The source does not establish that Google implemented every recommendation as company policy.

**Evidence limit.** This is qualitative self-report, not a causal estimate that AI slowed Google engineers or a measurement of how common every theme was. Separately, the article summarizes DORA's cross-organization association between increased AI adoption, increased delivery throughput and increased delivery instability. That aggregate association must not be relabeled as Google's internal result or proof of causation.

**Business lesson.** Measure the complete task, including review, rework and production readiness. Generated lines, accepted suggestions and tool usage are insufficient on their own.

### 2.3 GitLab: make responsibility and autonomy explicit

**The challenge.** GitLab's public engineering guidance says AI output can be confidently wrong. Its infrastructure principles explicitly recognize the cost imposed on reviewers and on-call engineers when generated work is not adequately understood or verified. Its AI-assisted development playbook warns that raising autonomy before the surrounding engineering system is ready can produce unreliable output and amplify technical debt. [S3](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/946c9f1441d92caa142091e0678e7dbdac3d38c3/content/handbook/engineering/infrastructure-platforms/developer-experience/ai/_index.md) [S4](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/5f92de4547bca68f41f5ec784e621f097c1e8b38/content/handbook/engineering/workflow/ai-assisted-development.md) [S7](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/844ac1c774b21fa1e7b50c2c164e02de82b417d6/content/handbook/engineering/infrastructure-platforms/ai_usage_principles.md)

**What GitLab chose.** The DevEx team documents using AI tools while retaining normal code review, prohibiting confidential/customer/unreleased information in external AI tools, and expecting merge-request authors to label their level of AI assistance. Its guidance favors deterministic tools such as linters where they are cheaper and faster than duplicating checks with AI. The playbook describes maturity gates around CI, context/documentation, tests and review before increasing autonomy.

**Evidence limit.** These are published team practices and engineering standards, not verified company-wide adoption rates or quantified savings. GitLab's employee general-purpose AI requirements include an internal-only document that was not accessed; this report does not invent its contents.

**Business lesson.** Assign ownership of generated work, communicate how AI was used, preserve review standards and match autonomy to demonstrated engineering readiness.

### 2.4 Microsoft: approval and MCP permissions require patch management

**The challenge.** On October 13, 2026, Microsoft published two VS Code security advisories relevant to agentic coding:

- **CVE-2026-102232:** an affected Copilot agent could be influenced into editing enabled custom hook or agent-definition files without the intended approval. A subsequently invoked hook could execute a command with the user's privileges. [S5](https://github.com/microsoft/vscode/security/advisories/GHSA-fq62-m6f5-c7h9)
- **CVE-2026-102851:** network-access and filesystem-write permissions approved for one MCP server could be shared with another server using the same sandbox configuration. [S6](https://github.com/microsoft/vscode/security/advisories/GHSA-qghm-w43w-vx8v)

**What Microsoft changed.** Version 1.141.1 adds confirmation for edits to the affected sensitive locations. It also scopes MCP grants to individual servers, restricts shared configuration to deny rules and ignores legacy shared grants.

**Evidence limit.** These are documented vulnerabilities and fixes. The advisories do not establish exploitation in the wild, identify a customer breach or quantify losses.

**Business lesson.** Govern agent clients, plugins, hooks and MCP servers as security-sensitive software. Approval settings alone are insufficient without version ownership, patching, permission scoping and regression checks.

### 2.5 Anthropic and GitHub: constrain the agent's authority

**The challenge.** Untrusted content can influence tools with access to files, credentials and networks. Anthropic's sandbox-runtime documentation explicitly identifies the need for both filesystem and network isolation. It warns that broad access to an allowed domain, a host Docker socket or writable execution paths can undermine isolation. [S8](https://github.com/anthropic-experimental/sandbox-runtime/blob/main/README.md)

**What the providers chose.** Anthropic implements OS-enforced filesystem/network restrictions around processes and their children. GitHub's cloud-agent documentation describes constrained repository and branch access, specially scoped secrets, human workflow gates, signed changes and session evidence. Its firewall documentation explicitly states residual risks and limits direct coverage for MCP server processes and setup steps. [S9](https://github.com/github/docs/blob/main/content/copilot/responsible-use/agents.md) [S10](https://github.com/github/docs/blob/main/content/copilot/how-tos/copilot-on-github/customize-copilot/customize-the-firewall.md)

**Evidence limit.** These are provider product-design responses, not proof of named-customer deployment, complete protection or a reported customer incident. Anthropic's referenced runtime is a beta research preview. The point is the control pattern, not a recommendation to deploy that package without qualification.

**Business lesson.** Control the agent's actual authority and routes. Review the coverage of each tool path; an approved model or a firewall label does not establish that every integration is governed.

### 2.6 Shopify: inspect the data flows around the model

**The challenge.** An AI workflow can transmit information through plugins, validation tools and telemetry as well as its main model call. Shopify's official AI Toolkit README documents telemetry enabled by default. Depending on the invocation/capture path, it can include search text, validated code and recent user-prompt content. [S11](https://github.com/Shopify/Shopify-AI-Toolkit/blob/main/README.md)

**What Shopify provides.** Its documentation identifies the collection surfaces and supplies opt-out mechanisms, including a user-level file and environment settings. This is disclosed product behavior, not an allegation of a breach, malicious collection or improper employee use.

**Business lesson.** An approved LLM gateway does not automatically govern every data recipient in an agent's ecosystem. Review extension behavior, telemetry, auto-updates and opt-out enforcement before distributing tools to employees.

## 3. The risks of expanding without an operating plan

The following are foreseeable operating risks and recommendations synthesized from the evidence. They are not claims that every cited company suffered every problem.

| Risk | What can go wrong | Required planning decision |
|---|---|---|
| Data and credential exposure | Code, documents, tool results or telemetry reach an unintended provider; credentials become readable to an agent. | Approved destinations/data classes; credential isolation; complete data-flow inventory; defined inspection coverage. |
| Excessive agent authority | Prompt injection, mistakes or shared permissions produce unauthorized actions. | Per-user/workload/tool permissions; constrained targets; sensitive-action approvals; patch ownership. |
| Quality and operational instability | Plausible code passes superficial review but fails during integration or production operation. | Testing, review, provenance, production-readiness criteria and rollback ownership. |
| Uncontrolled total cost | Retries, long contexts, background tasks, idle environments and review work consume more than expected. | Attribution, budgets, run/resource limits, lifecycle cleanup and outcome-based accounting. |
| Poor end-to-end performance | Fast generation is offset by slow setup, retrieval, verification, queues or review. | Task-level baselines and latency/quality measures across the complete workflow. |
| Fragmented employee experience | Each employee independently assembles models, plugins, tools and environments. | Supported configurations, training, clear defaults and a path for legitimate exceptions. |
| Stale or over-shared context | Retained history, memory or embeddings outlive access or preserve incorrect information. | Source ownership, access propagation, provenance, correction, retention and derived-data deletion. |
| Incomplete incident response | The company cannot identify affected actions, revoke access or stop a running agent. | Correlated evidence, scoped containment, revocation, recovery and incident owners. |
| Vendor and configuration drift | Model, client, plugin or provider changes invalidate tested assumptions. | Version/change inventory, compatibility evaluation, staged rollout and exit/portability requirements. |

### 3.1 Security must extend beyond a warning in the prompt

Instructions are useful context, but they do not remove filesystem permissions, revoke tokens or isolate MCP grants. A plan should independently govern identity, accessible resources, actions, data destinations and retained information.

Keep long-lived provider and privileged backend credentials outside model-visible workspaces where possible. When an agent can run arbitrary shell with the same access as a user, it can generally read the credentials available to that user. Secret scanning is defense in depth; it cannot guarantee recognizing every arbitrary password, encoded value or newly returned secret.

Likewise, an external safety or decision model is itself an external data recipient. A company cannot send prohibited content to a remote evaluator to decide whether that content may leave the company. Local/cloud/hybrid policy must cover all relevant processing, including summaries, embeddings, retrieval services, guardrail models, plugins and telemetry.

### 3.2 Costs require a complete business case

An AI seat price or a per-token price is only one cost. The company should budget for licenses, inference, tool calls, retries, environment compute/storage, local-model capacity, context/memory processing, evaluations, observability, integration, training, review/rework and operations.

Google Cloud DORA's published ROI framework explicitly separates tooling, enablement and infrastructure costs from potential capacity, revenue and operational effects. Its calculator is a planning model, not a measured industry saving. [S12](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/ai/roi/report/index.md)

Two distinctions are essential:

- **Capacity is not cash savings.** Time made available is valuable only if it is used for an organizational outcome; salary-valued time is not automatically money removed from expenditure.
- **A budget alert is not a hard cap.** In-flight requests, shared counters, retries, unknown pricing and local resource use affect enforcement. Define acceptable overshoot and outage behavior.

A useful economic unit is **total cost per accepted, verified outcome**, with quality and reliability measured alongside it. More generated code or more tokens are activity, not proof of value. This report makes no unsupported claim about a named company's AI spending overrun or quantified inference-cost saving.

### 3.3 Performance and productivity must be measured locally

The independent research organization METR published a narrow early-2025 study of experienced open-source developers. Its official data/reproduction repository contains 246 tasks across 16 developers and reports approximately **19% more completion time with AI** in that setting. This is not a claim about all developers or current 2026 tools. [S13](https://github.com/METR/Measuring-Early-2025-AI-on-Exp-OSS-Devs)

That historical result and Accenture's reported positive enterprise comparison are not contradictory universal estimates. Their populations, tasks, tools, methods and reported outcomes differ. Together they justify task-specific pilots instead of assuming a fixed productivity multiplier.

Measure time to a useful result through environment preparation, context gathering, generation, testing, review, rework and production integration. Segment familiar/unfamiliar code, routine/complex tasks, and differing levels of developer experience. Track model/client versions so a new configuration is not treated as the same intervention.

### 3.4 People and accountability are part of the system

Employees need a supported path, understandable restrictions and a way to request exceptions. Blanket availability without guidance can produce incompatible toolchains and unclear responsibility. Restrictions without usable alternatives can encourage workarounds.

Retain an accountable human owner for generated changes. Train reviewers to assess evidence and risk rather than trusting plausible prose or requiring an arbitrary degree of manual rewriting. Match scrutiny to impact, and account for reviewer and on-call capacity. GitLab's published principles provide a concrete example of this proportional approach. [S7](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/844ac1c774b21fa1e7b50c2c164e02de82b417d6/content/handbook/engineering/infrastructure-platforms/ai_usage_principles.md)

## 4. What a credible company plan must contain

### A. A business scope and an accountable owner

Name the initial use cases, employees/projects, permitted data/actions, intended benefit and success measures. Identify who accepts the residual risk. Separate advisory assistance, sandbox execution, staging changes and production-affecting automation.

### B. Approved capabilities and effective configurations

Maintain supported combinations of model, agent client, environment, context/memory, tools/MCP and skills. Record owners, versions, permissions, limitations and data recipients. Validate the combination rather than approving each component independently and assuming compatibility.

### C. Identity, data and action boundaries

Connect company identity to project entitlements and service/workload identity. Keep access narrowly scoped and revocable. Specify eligible internal/external destinations, credential placement and required inspections. Require independent authorization and appropriate human approval for consequential actions.

### D. A measured pilot and staged autonomy

Establish baselines, collect representative task results and evaluate both benefit and harm. Retain normal software-delivery checks. Increase autonomy only when context, tests, CI, review and incident processes support it. Re-evaluate changes to models, tools, skills and policies.

### E. Cost and capacity controls

Assign spend/resource ownership and track total cost. Set limits on run duration/steps, concurrency, model usage, environment resources and background work. Define idle cleanup, budget escalation and behavior when limits or accounting services fail.

### F. Evidence, privacy and incident response

Correlate the employee, environment, task, model/tool action, applicable policy, approval and result. Collect the minimum content needed; full prompts, completions and embeddings should not be logged indiscriminately. Define who may inspect evidence and its retention/deletion.

Plan to suspend a tool/provider, stop a task, revoke credentials, patch clients, preserve authorized evidence and restore service. Offboarding must cover active tasks and issued credentials as well as future login access.

### G. Training and a supported exception path

Teach employees how to select approved capabilities, verify output, handle confidential information, interpret denials, report incidents and request legitimate changes. Publish responsibility for source/code review, knowledge freshness, approvals and operational ownership.

## 5. Recommended measures for leadership

| Dimension | Useful measures | Misleading shortcut |
|---|---|---|
| Business value | Accepted useful outcomes; delivery/customer results attributable to the use case | Generated lines or subscription count |
| Productivity | End-to-end task time, reviewer effort, rework and developer experience | Faster first draft alone |
| Quality/reliability | Test/build success, escaped defects, change failures and incident impact | Plausible output or confidence score |
| Cost | Full cost per verified outcome; spend/resource attribution; idle/retry waste | Token price alone |
| Security | Defined test coverage, authorization failures, control bypasses and revocation completion | Number of blocked prompts alone |
| Adoption | Time to first useful authorized task; friction; exception resolution | Mandatory use as evidence of benefit |
| Governance | Supported/qualified configurations, policy version coverage and accountable ownership | A written policy without verified enforcement |

Set targets using local baselines and consequences. Avoid importing a vendor's productivity percentage or a public calculator's defaults as the company's forecast.

## 6. Relevance to a company-controlled AI work platform

The evidence supports a need for coherent administration across providers, employee environments, context/memory, agents, tools, security checks and operating evidence. A central application could make supported configurations easier to publish and use, apply consistent rules, attribute spending and connect an event to its owner and policy.

It must still demonstrate its enforcement coverage and value. A model gateway alone does not manage every credential, plugin or tool path. A memory connector alone does not implement source authorization and deletion. A policy editor alone does not establish that a rule is applied. An AI classifier's score does not supply permission or human approval.

The product opportunity is to make an adoption plan **operational, understandable and measurable**. The cited cases justify the problem and control patterns; they do not prove that a particular new product is necessary, unique, sufficient or better than existing alternatives.

## Conclusion

Companies need an AI coding and agent adoption plan because these tools change the flow of information, the authority of software, the economics of engineering and the distribution of human work. Public company evidence shows the importance of controlled rollout, evaluation, identity, software security, scoped execution, review and accountability.

A credible plan gives employees a reliable way to use AI and gives the company evidence that the resulting work is useful, authorized, affordable and supportable. It should evolve as models, tools and operating experience change.

## References and evidence notes

All sources were inspected on October 21, 2026. Publication dates below are only those established by the source. Repository snapshots without a clear publication date are labeled accordingly. Links are to first-party sources except METR, which is the primary author of its own research. Some rendered sites were blocked by the execution environment; official GitHub/GitLab sources were used. No inaccessible article was cited as if it had been read.

**S1 — Accenture / GitHub.** *Accenture customer story.* Publication date not exposed; accessed October 21, 2026. Vendor/customer account of pilot, controlled comparison, rollout and platform choices. Outcome details are reported rather than independently audited. [Source](https://github.com/customer-stories/accenture).

**S2 — Jessica Baolin and Nathen Harvey, Google Cloud DORA.** *Balancing AI tensions: Moving from AI adoption to effective SDLC use.* March 10, 2026. Includes qualitative Google engineer responses and separately discusses cross-organization DORA associations. [Pinned source](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/insights/balancing-ai-tensions/index.md).

**S3 — GitLab DevEx.** *AI in Developer Experience.* Inspected file last changed March 16, 2026; that is not an asserted original publication date. Team practices, disclosure labels, confidentiality and review guidance. [Pinned source](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/946c9f1441d92caa142091e0678e7dbdac3d38c3/content/handbook/engineering/infrastructure-platforms/developer-experience/ai/_index.md).

**S4 — GitLab.** *AI-Assisted Development Playbook.* Inspected file last changed October 13, 2026. Engineering standards/maturity guidance; not a quantified outcome study. [Pinned source](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/5f92de4547bca68f41f5ec784e621f097c1e8b38/content/handbook/engineering/workflow/ai-assisted-development.md).

**S5 — Microsoft.** *Remote Code Execution via Custom Hook Edits in the Copilot Harness.* October 13, 2026. GHSA-fq62-m6f5-c7h9 / CVE-2026-102232. Disclosed vulnerability and fix; no exploitation claim. [Advisory](https://github.com/microsoft/vscode/security/advisories/GHSA-fq62-m6f5-c7h9).

**S6 — Microsoft.** *Security Feature Bypass via Shared MCP Sandbox Permission Approvals.* October 13, 2026. GHSA-qghm-w43w-vx8v / CVE-2026-102851. Disclosed vulnerability and fix; no exploitation claim. [Advisory](https://github.com/microsoft/vscode/security/advisories/GHSA-qghm-w43w-vx8v).

**S7 — GitLab Infrastructure Platforms.** *AI Usage Principles.* Inspected file last changed April 16, 2026. Internal team principles on responsibility, impact, review and on-call load. [Pinned source](https://gitlab.com/gitlab-com/content-sites/handbook/-/blob/844ac1c774b21fa1e7b50c2c164e02de82b417d6/content/handbook/engineering/infrastructure-platforms/ai_usage_principles.md).

**S8 — Anthropic.** *sandbox-runtime README.* Current repository documentation; publication date not established. Beta research preview with explicit security limitations. Product design, not a customer case. [Source](https://github.com/anthropic-experimental/sandbox-runtime/blob/main/README.md).

**S9 — GitHub.** *Agents responsible-use/application documentation.* Current documentation; publication date not established. Product controls and limitations, not proof of customer outcomes. [Source](https://github.com/github/docs/blob/main/content/copilot/responsible-use/agents.md).

**S10 — GitHub.** *Customize the cloud-agent firewall.* Current documentation; publication date not established. Includes coverage limitations for MCP servers and setup steps. [Source](https://github.com/github/docs/blob/main/content/copilot/how-tos/copilot-on-github/customize-copilot/customize-the-firewall.md).

**S11 — Shopify.** *Shopify AI Toolkit README: Telemetry and opting out.* Current repository documentation; publication date not established. Documents collection/opt-out behavior; not an incident or employee-rollout case. [Source](https://github.com/Shopify/Shopify-AI-Toolkit/blob/main/README.md).

**S12 — Google Cloud DORA.** *AI ROI framework and calculator.* Report page published April 9, 2026; updated April 22, 2026. Planning model, not realized savings or an industry cost average. [Report source](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/ai/roi/report/index.md); [calculation implementation](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/svelte/roi-calculator/src/lib/calculations.js).

**S13 — METR.** *Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity.* July 2025. Official data/reproduction repository; historical narrow randomized study. No extrapolation to all tasks/current tools. [Repository and methods](https://github.com/METR/Measuring-Early-2025-AI-on-Exp-OSS-Devs).

**Additional source context — Google Cloud DORA.** *State of AI-assisted Software Development 2025.* September 15, 2025. Industry research summary describes AI as an amplifier of organizational strengths/weaknesses. Full gated report not retrieved; no additional coefficients or sample sizes inferred. [Source](https://github.com/dora-team/dora.dev/blob/b14ae080c350ca7ff449889621a970e959203bd5/hugo/content/research/2025/dora-report/index.md).
