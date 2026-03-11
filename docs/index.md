---
icon: lucide/rocket
---

# Automate PoC

Agentic Plugins that help Sales Engineers set up, configure, and troubleshoot PoCs in prospect environments faster and more accurately — so they can win more deals.


[:material-frequently-asked-questions: Read the FAQ](faq.md){ .md-button }

---

## Demo
<i>100-second video coming soon.</i>

---

## Get started

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

<!-- ### Step 3: Add plugins to your agentic coding tool

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

    <i>Planning to add support for others such as Gemini CLI, Codex, etc.</i> -->


<!-- ## 5 minutes to try a demo
<i>Coming soon... using stackblitz, codesandbox, or similar for you to try a demo.</i> -->