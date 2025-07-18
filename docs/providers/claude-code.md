---
sidebar_label: Claude Code
---

# Using Claude Code With Kilo Code

Claude Code is Anthropic's official CLI that provides direct access to Claude models from your terminal. Using Claude Code with Kilo Code lets you leverage your existing CLI setup without needing separate API keys.

**Website:** [https://docs.anthropic.com/en/docs/claude-code/setup](https://docs.anthropic.com/en/docs/claude-code/setup)

## Installing and Setting Up Claude Code

1. **Install Claude Code:** Follow the installation instructions at [Anthropic's Claude Code documentation](https://docs.anthropic.com/en/docs/claude-code/setup).
2. **Authenticate:** Run `claude` in your terminal. Claude Code offers multiple authentication options including the Anthropic Console (default), Claude App with Pro/Max plans, and enterprise platforms like Amazon Bedrock or Google Vertex AI. See [Anthropic's authentication documentation](https://docs.anthropic.com/en/docs/claude-code/setup) for complete details.
3. **Verify Installation:** Test that everything works by running `claude --version` in your terminal.

## Supported Models

Kilo Code supports the following Claude models through Claude Code:

*   `claude-sonnet-4` (Recommended)
*   `claude-4-opus`

The specific models available depend on your Claude subscription and plan. See [Anthropic's Model Documentation](https://docs.anthropic.com/en/docs/about-claude/models) for more details on each model's capabilities.

## Configuration in Kilo Code

1. **Open Kilo Code Settings:** Click the gear icon (<Codicon name="gear" />) in the Kilo Code panel.
2. **Select Provider:** Choose "Claude Code" from the "API Provider" dropdown.
3. **Select Model:** Choose your desired Claude model from the "Model" dropdown.
4. **(Optional) Custom CLI Path:** If you installed Claude Code to a location other than the default `claude` command, enter the full path to your Claude executable in the "Claude Code Path" field. Most users won't need to change this.

## Tips and Notes

*   **No API Keys Required:** Claude Code uses your existing CLI authentication, so you don't need to manage separate API keys.
*   **Cost Transparency:** Usage costs are reported directly by the Claude CLI, giving you clear visibility into your spending.
*   **Advanced Reasoning:** Full support for Claude's thinking modes and reasoning capabilities when available.
*   **Context Windows:** Claude models have large context windows, allowing you to include significant amounts of code and context in your prompts.
*   **Custom Paths:** If you installed Claude Code in a non-standard location, you can specify the full path in the settings. Examples:
    *   Windows: `C:\tools\claude\claude.exe`
    *   macOS/Linux: `/usr/local/bin/claude` or `~/bin/claude`

## Troubleshooting

*   **"Claude Code process exited with error":** Verify Claude Code is installed (`claude --version`) and authenticated (`claude auth login`). Make sure your subscription includes the selected model.
*   **Custom path not working:** Use the full absolute path to the Claude executable and verify the file exists and is executable. On Windows, include the `.exe` extension.
