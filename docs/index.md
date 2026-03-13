---
icon: lucide/rocket
---

# Automate PoC

A process improvement using agentic CLI and plugins for easier, faster PoC setup, configuration, and troubleshooting.


[:material-frequently-asked-questions: Read the FAQ](faq.md){ .md-button }

---

## Demo
<i>100-second video coming soon.</i>

---

## Get started

### Step 1: Access to LLM
<i>Skip if you already have access to an LLM server.</i>

=== "Claude"

    <i>[Set up by your Sales Engineer](serf.md).</i>

=== "Local LLM"

    <i>Coming soon.</i>

### Step 2: Set up agentic CLI (for macOS / Linux)
<i>Skip if you already have an agentic coding tool (Codex, Gemini CLI, etc.).</i>

=== "Claude Code"

    For a full install, see <a href="https://code.claude.com/" target="_blank">code.claude.com</a>. Otherwise, use the portable setup below.

    ``` bash
    curl -fsSL https://claude.ai/install.sh | bash
    ```

    Start Claude Code

    ``` bash
    claude --settings '{"env":{"ANTHROPIC_BASE_URL":"YYY_PROVIDED_BY_YOUR_ASSIGNED_SALES ENGINEER_YYY","ANTHROPIC_AUTH_TOKEN":"YYY_PROVIDED_BY_YOUR ASSIGNED_SALES_ENGINEER_YYY"}}'
    ```

=== "OpenCode"

    For a full install, see <a href="https://opencode.ai/" target="_blank">opencode.ai</a>. Otherwise, use the portable setup below.

    Download the portable OpenCode script:
    ``` bash
    curl -fLO https://raw.githubusercontent.com/jek-bao-choo/opencode-fork/refs/heads/dev/opencode-portable.sh
    ```

    Make it executable:
    ``` bash
    chmod +x opencode-portable.sh
    ```

    Create the config file <i>(replace `YOUR_GATEWAY_URL` with the URL provided by your Sales Engineer)</i>:
    ``` bash
    cat << 'EOF' > opencode-config.json
    {
        "$schema": "https://opencode.ai/config.json",
        "provider": {
            "litellm": {
            "npm": "@ai-sdk/openai-compatible",
            "name": "LiteLLM",
            "options": {
                "baseURL": "YOUR_GATEWAY_URL/v1"
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

    Launch OpenCode:
    ``` bash
    OPENCODE_CONFIG="./opencode-config.json" ./opencode-portable.sh

    # Once OpenCode opens, run:
    #   /connect
    #
    # Search for and select:
    #   LiteLLM
    #
    # Enter the API key provided by your assigned Sales Engineer
    ```

    

### Step 3: Add the marketplace and plugins

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