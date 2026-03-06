---
icon: lucide/rocket
---

# Automate PoC for Sales Engineers

## Current & Future States

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
title: After (with Agentic Codin Plugins)
---
graph TD
  A["<b>1. Formulate Success Criteria,</b>
  <b>PoC Scope & Plan</b>
  from discovery notes
  <i></i>
  <i>⏱ 0.5 hrs</i>
  <i></i>  
  <i>GenAI Web UI / Agentic Coding with SE's SKILLS Plugin</i>"]
  B["<b>2. Validate Unfamiliar Tech Stack</b>
  Sandbox env, config & instrumentation
  Revise scope to Datadog strengths
  <i></i>
  <i>⏱ 12 hrs (4 days x 3 hrs)</i>
  <i></i>
  <i>Agentic Coding + SE's SKILLS Plugins</i>"]
  C["<b>3. Prospect Discussion & Sign-Off</b>
  Discuss scope, revise & agree
  <i></i>
  <i>⏱ 2 hrs (no change)</i>"]
  D["<b>4. Kick Off PoC</b>
  Hands-on evaluation & instrumentation
  <i></i>
  <i>⏱ 6 hrs (2 wks x 3 sessions x 1 hr)</i>
  <i></i>  
  <i>Agentic Coding + SE's SKILLS Plugins</i>
  <i></i>
  <i>*FAQ: See below for prospect concerns</i>"]
  E["<b>5. Troubleshooting</b>
  Debug misconfigurations
  Support ticket guidance
  <i></i>
  <i>⏱ 3 hrs (3 issues x 1 hr)</i>
  <i></i>
  <i>Agentic Coding with SE's SKILLS Plugin</i>"]
  F["<b>6. Read-Out Playback</b>
  Prepare final deck with Datadog data
  <i></i>
  <i>⏱ 2 hrs</i>
  <i></i>
  <i>Agentic Coding with Datadog MCP Server and SE's SKILLS Plugin</i>"]
  G(["<b>Total: ~25.5 hrs (~77% reduction)</b>"])
  A --> B --> C --> D --> E --> F --> G
  style A fill:#c8e6c9
  style B fill:#c8e6c9
  style D fill:#c8e6c9
  style E fill:#c8e6c9
  style F fill:#c8e6c9
  style G fill:#a5d6a7
```

</div>

## Get started now in 3 steps

=== "OpenCode"

    ``` bash
    pip install zensical
    ```

=== "Claude Code"

    ``` bash
    npm install zensical
    ```

## *FAQ