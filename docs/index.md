---
icon: lucide/rocket
---

# Automate PoC

A process improvement using agentic CLI and plugins for easier, faster PoC setup, configuration, and troubleshooting.


[:material-frequently-asked-questions: Read the FAQ](faq.md){ .md-button }

---

## Demo

*Viewable by organisation members only.*

**Setup walkthroughs**

- [Step 1 - 35s demo](https://drive.google.com/file/d/1YJ5KMXQnh95JYnE9R3POvuJ6y1guYNsC/view?usp=sharing){:target="_blank"}
- [Step 2 - 129s demo](https://drive.google.com/file/d/1H61MhhmHFkeBm-OZiv3zUrLgiO1tRfWb/view?usp=sharing){:target="_blank"}
- [Step 3 - 80s demo](https://drive.google.com/file/d/1l8fkX1jNgcNGVTnuCXiySIpNXHyVqkht/view?usp=sharing){:target="_blank"}

**Real-world example**

[Prospect troubleshooting missing APM traces with Project DateNight](https://drive.google.com/file/d/1PEEquQ_O8WagfdvbTUoJHrj6npOOZ3Xa/view?usp=sharing){:target="_blank"} (~12min) — see the [root cause and solution report](https://drive.google.com/file/d/1R6EVQzrXXtaQK5LeLQoNcwvx3m5Qhywi/view?usp=sharing){:target="_blank"} and [final outcome](https://drive.google.com/file/d/13R_uyxq8t09LDYQuDDeEjWo0AS2qfvd1/view?usp=sharing){:target="_blank"}. The Sales Engineer resolved the issue and got tracing working faster than expected, within an hour, without raising a support ticket.

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

    **Download and install <a href="https://code.claude.com/" target="_blank">Claude Code</a>:**

    ``` bash
    curl -fsSL https://claude.ai/install.sh | bash
    ```

    **Start Claude Code:** <i>(replace `YOUR_GATEWAY_BASE_URL` and `YOUR_API_KEY` **provided by your Sales Engineer**)</i>

    Option 1 — settings flag (inline config)
    ``` bash
    ~/.local/bin/claude --settings '{"env":{"ANTHROPIC_BASE_URL":"YOUR_GATEWAY_BASE_URL","ANTHROPIC_AUTH_TOKEN":"YOUR_API_KEY"}}'
    ```

    Option 2 — environment variables (temporary, current session only)
    ``` bash
    ANTHROPIC_BASE_URL="YOUR_GATEWAY_BASE_URL" ANTHROPIC_AUTH_TOKEN="YOUR_API_KEY" ~/.local/bin/claude
    ```



=== "OpenCode"

    For a full install, see <a href="https://opencode.ai/" target="_blank">opencode.ai</a>. Otherwise, use the portable setup below.

    **Download the portable OpenCode script:**
    ``` bash
    curl -fLO https://raw.githubusercontent.com/jek-bao-choo/opencode-fork/refs/heads/dev/opencode-portable.sh
    ```

    **Make it executable:**
    ``` bash
    chmod +x opencode-portable.sh
    ```

    **Create the config file:** <i>(replace `YOUR_GATEWAY_BASE_URL` **provided by your Sales Engineer**)</i>
    ``` bash
    cat << 'EOF' > opencode-config.json
    {
        "$schema": "https://opencode.ai/config.json",
        "provider": {
            "litellm": {
            "npm": "@ai-sdk/openai-compatible",
            "name": "LiteLLM",
            "options": {
                "baseURL": "YOUR_GATEWAY_BASE_URL/v1"
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