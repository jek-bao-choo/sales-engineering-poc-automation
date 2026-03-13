# FAQ

<details open markdown>
<summary><b>What is Project DateNight?</b></summary>

Project DateNight helps Sales Engineers run PoCs in prospect environments using agentic CLI and plugins for easier, faster PoC setup, configuration, and troubleshooting.

</details>

<details markdown>
<summary><b>Why Project DateNight?</b></summary>

Project DateNight improves SE productivity by more than 50%. Compare a typical PoC workflow before and after:

<div class="grid" markdown>

``` mermaid
---
title: Before
---
graph TD
  A["<b>1. Formulate Success Criteria,</b>
  <b>PoC Scope & Plan</b>
  from discovery notes
  <i></i>
  <i>⏱ 2 hrs</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>"]
  B["<b>2. Validate Unfamiliar Tech Stack</b>
  Sandbox env, config & instrumentation
  Revise scope to Datadog strengths
  <i></i>
  <i>⏱ 60 hrs (10 days x 6 hrs)</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>"]
  C["<b>3. Prospect Discussion & Sign-Off</b>
  Discuss scope, revise & agree
  <i></i>
  <i>⏱ 2 hrs</i>"]
  D["<b>4. Kick Off PoC</b>
  Guided hands-on evaluation
  Config, instrumentation, status updates
  <i></i>
  <i>⏱ 36 hrs (4 wks x 3 sessions x 3 hrs)</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>"]
  E["<b>5. Troubleshooting</b>
  Debug misconfigurations
  Guide on flare & support tickets
  <i></i>
  <i>⏱ 6 hrs (3 issues x 2 hrs)</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>"]
  F["<b>6. Read-Out Playback</b>
  Prepare final deck with Datadog data
  <i></i>
  <i>⏱ 4 hrs</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>
  <i>&nbsp;</i>"]
  G(["<b>Total: ~110 hrs</b>"])
  A --> B --> C --> D --> E --> F --> G
```

``` mermaid
---
title: After (with Agentic Plugins)
---
graph TD
  A["<b>1. Formulate Success Criteria,</b>
  <b>PoC Scope & Plan</b>
  from discovery notes
  <i></i>
  <i>⏱ 0.5 hrs</i>
  <i></i>
  <i>GenAI Web UI or Agentic Coding + Agentic Plugins</i>"]
  B["<b>2. Validate Unfamiliar Tech Stack</b>
  Sandbox env, config & instrumentation
  Revise scope to Datadog strengths
  <i></i>
  <i>⏱ 12 hrs (4 days x 3 hrs)</i>
  <i></i>
  <i>Agentic Coding + Agentic Plugins</i>"]
  C["<b>3. Prospect Discussion & Sign-Off</b>
  Discuss scope, revise & agree
  <i></i>
  <i>⏱ 2 hrs (no change)</i>"]
  D["<b>4. Kick Off PoC</b>
  Hands-on evaluation & instrumentation
  <i></i>
  <i>⏱ 6 hrs (2 wks x 3 sessions x 1 hr)</i>
  <i></i>
  <i>Agentic Coding + Agentic Plugins</i>
  <i></i>
  <i>*FAQ: See below for prospect concerns</i>"]
  E["<b>5. Troubleshooting</b>
  Debug misconfigurations
  Support ticket guidance
  <i></i>
  <i>⏱ 3 hrs (3 issues x 1 hr)</i>
  <i></i>
  <i>Agentic Coding with Agentic Plugins</i>"]
  F["<b>6. Read-Out Playback</b>
  Prepare final deck with Datadog data
  <i></i>
  <i>⏱ 2 hrs</i>
  <i></i>
  <i>Agentic Coding with Datadog MCP Server and Agentic Plugins</i>"]
  G(["<b>Total: ~25.5 hrs (~77% productivity improvement)</b>"])
  A --> B --> C --> D --> E --> F --> G
  style A fill:#c8e6c9,color:#1a1a1a
  style B fill:#c8e6c9,color:#1a1a1a
  style D fill:#c8e6c9,color:#1a1a1a
  style E fill:#c8e6c9,color:#1a1a1a
  style F fill:#c8e6c9,color:#1a1a1a
  style G fill:#a5d6a7,color:#1a1a1a
```

</div>

</details>

<details markdown>
<summary><b>Why is it called Project DateNight?</b></summary>

The project creator spent nights (sometimes date nights) building these plugins so other Sales Engineers don't have to sacrifice theirs.

Other names considered:

- Project SE AI Toolkit
- Project SE PoC Automation
- Project Agentic Plugins

It's just a project name for now; what matters is whether it improves PoC productivity.

</details>

<details markdown>
<summary><b>How do I collaborate?</b></summary>

Collaborators are welcome. This project will only thrive with collaboration. 

Project DateNight is intended to be built by Sales Engineers for Sales Engineers — a community driven project. Please contact Jek Bao.

</details>

<details markdown>
<summary><b>Are my prospects' data used to train Claude models?</b></summary>

Usage follows the company usage policy, and Claude doesn't train on the data under the Enterprise plan.

</details>

<details markdown>
<summary><b>Why get a Claude API key through Project DateNight instead of directly?</b></summary>

Project DateNight tracks spending, enforces key expiration, and tags keys to sales opportunities - so prospects use the key for the PoC.

</details>
