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

    If you prefer to [install OpenCode](https://opencode.ai/) otherwise follow the step below for no installation, portable OpenCode.
    
    macOS / Linux:
    ``` bash
    curl -fLO https://raw.githubusercontent.com/jek-bao-choo/opencode-fork/refs/heads/dev/opencode-portable.sh
    ```

    ``` bash
    chmod +x opencode-portable.sh
    ```

    ``` bash
    cat << 'EOF' > opencode-config.json
    {
        "$schema": "https://opencode.ai/config.json",
        "provider": {
            "litellm": {
            "npm": "@ai-sdk/openai-compatible",
            "name": "LiteLLM",
            "options": {
                "baseURL": "THE_SALES_ENGINEER_MUST_CHANGE_THIS_GATEWAY_URL/v1"
            },
            "models": {
                "claude-opus-4-6": {
                "name": "Claude Opus 4.6"
                },
                "claude-sonnet-4-6": {
                "name": "Claude Sonnet 4.6"
                }
            }
            }
        }
    }
    EOF
    ```

    ``` bash
    OPENCODE_CONFIG="./opencode-config.json" ./opencode-portable.sh

    # Then inside of OpenCode type in
    # /connect
    # 
    # Next search for 
    # LiteLLM
    #
    # Enter the key (The Sales Engineer will provide the key)
    ```

    

### Step 3: Add the LLM key, marketplace, and plugin(s)

=== "Claude Code"

    Add [the marketplace](https://github.com/jek-bao-choo/datadog-agentic-plugins)

    ``` bash
    /plugin marketplace add https://github.com/jek-bao-choo/datadog-agentic-plugins
    ```

    Install the plugin

    ``` bash
    /plugin install quickstart@datadog-agentic-plugins
    ```

    Reload the plugins

    ``` bash
    /reload-plugins
    ```

    Display the menu

    ```bash
    /quickstart:menu
    ```

=== "OpenCode"

    <i>Coming soon.</i>

=== "Others"

    <i>Planning to add support for others such as Gemini CLI, Codex, etc.</i>


<!-- ## 5 minutes to try a demo
<i>Coming soon... using stackblitz, codesandbox, or similar for you to try a demo.</i> -->