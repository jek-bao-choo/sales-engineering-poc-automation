---
icon: lucide/rocket
---

# Automate PoC

## 70% productivity gain in Sales Engineering PoC process

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

## 100-second demo on setup and AI-assisted instrumentation
<i>Coming soon...</i>

## 3 steps to get started

### Step 1: Access to LLM
<i>Skip this step if you have access to your company's LLM server.</i>

=== "Claude"

    <i>Your assigned Sales Engineer will [set this up for you](serf.md).</i>

=== "Local LLM"

    <i>Coming soon.</i>

### Step 2: Set up agentic coding tool
<i>Skip this step if you have an existing agentic coding tool (Codex, Gemini CLI, etc.).</i>

=== "Claude Code (installation)"

    [macOS / Linux](https://code.claude.com/docs/en/quickstart#step-1-install-claude-code)

    ``` bash
    curl -fsSL https://claude.ai/install.sh | bash
    ```

    Start Claude Code

    ``` bash
    claude --settings '{"env":{"ANTHROPIC_BASE_URL":"YYY_PROVIDED_BY_YOUR_ASSIGNED_SALES ENGINEER_YYY","ANTHROPIC_AUTH_TOKEN":"YYY_PROVIDED_BY_YOUR ASSIGNED_SALES_ENGINEER_YYY"}}'
    ```

=== "OpenCode (no installation, portable)"

    macOS / Linux:

    ``` bash
    curl -fLO https://raw.githubusercontent.com/jek-bao-choo/opencode-fork/refs/heads/dev/opencode-portable.sh
    ```

    ``` bash
    chmod +x opencode-portable.sh
    ```

### Step 3: Add plugins to your agentic coding tool

=== "Claude Code"

    ``` bash
    # git ...
    ```


    ```bash
    # claude --...
    ```

=== "OpenCode"

    ``` bash
    # git ...
    ```


    ```bash
    # ./opencode ---...
    ```

=== "Others"

    <i>Planning to add support for others such as Gemini CLI, Codex, etc.</i>


<!-- ## 5 minutes to try a demo
<i>Coming soon... using stackblitz, codesandbox, or similar for you to try a demo.</i> -->