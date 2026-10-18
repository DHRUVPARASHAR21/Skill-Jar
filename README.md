# Skill Jar

A personal collection of reusable Codex skills.

Each skill is stored in its own folder under `skills/` and contains a `SKILL.md` manifest with its purpose, activation guidance, and workflow instructions. Some skills also include an `agents/openai.yaml` file with UI metadata.

## Included skills

| Skill | Purpose |
| --- | --- |
| [`idea-to-project`](skills/idea-to-project/) | Turns an explored idea, brief, or research notes into reviewable project groundwork before implementation. |

## Use a skill locally

Copy or clone the chosen skill folder into your Codex skills directory:

```text
~/.codex/skills/<skill-name>/
```

On Windows, this is normally:

```text
C:\Users\<your-user>\.codex\skills\<skill-name>\
```

Restart or open a new Codex session, then invoke a skill explicitly with `$skill-name` when useful. Codex can also select skills automatically when the request matches their descriptions.

## Adding a skill

1. Create a focused skill in `skills/<skill-name>/`.
2. Include a `SKILL.md` with valid YAML front matter containing `name` and `description`.
3. Add references, scripts, or assets only when they materially support the workflow.
4. Validate it with Codex's `skill-creator` validator before committing.
5. Add the skill to the table above.

Keep each skill narrow: use it for a repeatable workflow or policy, not as a catch-all set of instructions.
