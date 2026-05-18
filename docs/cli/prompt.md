
<!-- SPDX-FileCopyrightText: 2026 Apoorv Garg <apoorvgarg.21@gmail.com> -->
<!-- SPDX-License-Identifier: AGPL-3.0-only -->

# observal prompt

Manage reusable prompts in the registry.

Prompts are reusable templates that can be rendered with variables, installed into supported IDEs, and shared through the Observal registry.

## Subcommands

| Command | Description |
| --- | --- |
| [`prompt submit`](#observal-prompt-submit) | Submit a new prompt for review |
| [`prompt list`](#observal-prompt-list) | List approved prompts |
| [`prompt my`](#observal-prompt-my) | List your own prompts |
| [`prompt show`](#observal-prompt-show) | Show prompt details |
| [`prompt render`](#observal-prompt-render) | Render a prompt template with variables |
| [`prompt install`](#observal-prompt-install) | Get install config for a prompt |
| [`prompt edit`](#observal-prompt-edit) | Edit an existing prompt |
| [`prompt delete`](#observal-prompt-delete) | Delete a prompt |

---

## `observal prompt submit`

Submit a new prompt to the registry for review and approval.

```bash
observal prompt submit
```

Prompts can include template variables and metadata that allow them to be reused across agents and IDE integrations.

---

## `observal prompt list`

List all approved prompts available in the registry.

```bash
observal prompt list
```

Use this command to browse reusable prompts published by the community.

---

## `observal prompt my`

List prompts created by the authenticated user, including drafts and pending submissions.

```bash
observal prompt my
```

Useful for managing your own prompt submissions and checking review status.

---

## `observal prompt show`

Display detailed information about a specific prompt.

```bash
observal prompt show <id-or-name>
```

Shows metadata, template variables, author information, and installation details.

---

## `observal prompt render`

Render a prompt template using variables.

```bash
observal prompt render <id-or-name>
```

Use this command to preview the final rendered prompt before installation or usage.

---

## `observal prompt install`

Get installation configuration for a prompt.

```bash
observal prompt install <id-or-name>
```

This command outputs configuration snippets that can be used in supported IDEs and agent workflows.

---

## `observal prompt edit`

Edit an existing draft, pending, or rejected prompt.

```bash
observal prompt edit <id-or-name>
```

Allows updating metadata, variables, descriptions, and prompt content before approval.

---

## `observal prompt delete`

Delete a prompt from the registry.

```bash
observal prompt delete <id-or-name> [--yes]
```

Use `--yes` to skip the confirmation prompt.

---

## Related

* [`observal agent`](agent.md) — bundle prompts into installable agents
* [`observal registry`](registry.md) — manage registry resources
* [Use Cases → Share agent configs](../use-cases/share-agent-configs.md)