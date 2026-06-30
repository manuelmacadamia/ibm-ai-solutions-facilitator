# IBM AI Solutions Facilitator

Repository for configuring an AI assistant designed to facilitate an AI Solutions Canvas workshop, inspired by human-centered AI design practices, Enterprise Design Thinking, and AI Essentials.

The package is platform-agnostic: it can be used with ChatGPT, Gemini, or Claude, as long as the platform allows users to set instructions and upload source files.

## Language Behavior

The default language is English. At the beginning of every new workshop, the agent must first ask, in English:

```text
Which language would you like to use for this workshop? You can answer in any language.
```

After that, the agent continues in the language chosen by the user. If the answer is absent or ambiguous, it continues in English.

## What The Assistant Does

- Guides one complete workshop flow.
- Progressively builds an AI Solutions Canvas.
- Adapts to mixed AI skill levels.
- Produces a final playback, decision and workbook.
- If the platform supports file creation, can also produce printable HTML/PDF.

## Quick Setup

1. Create a new assistant/project/gem in your platform:
   - ChatGPT: Project or Custom GPT.
   - Gemini: Gem.
   - Claude: Project.
2. Open the instruction/system prompt area.
3. Copy the full content of `system_prompt.txt` into the instructions.
4. Upload the source files listed in `source_file_checklist.md`.
5. If available, enable file creation / code execution / data analysis tools.
6. Start with:

```text
/start
```

or:

```text
Guide me through the AI Solutions Canvas workshop.
```

## Which Files Matter

Not every file has the same role.

| File or folder | Role | Upload as source? |
|---|---|---|
| `system_prompt.txt` | Main instruction prompt. Copy this into the assistant instructions. | No, copy into instructions |
| `agent_profile.md` | Defines the facilitator identity and tone. | Yes |
| `orchestrator_operating_model.md` | Explains how the assistant runs the workshop. | Yes |
| `skill_manifest.md` | Maps workshop moments to skills. | Yes |
| `skills/` | Modular workshop skills. These are the operational core. | Yes |
| `templates/` | Canvas state, final workbook and HTML/PDF output format. | Yes |
| `examples/starter_prompts.md` | Test prompts for checking behavior. | Optional |
| `source_file_checklist.md` | Human checklist for setup. | No |
| `README.md` | GitHub documentation. | No |
| `.gitignore`, `LICENSE` | Repository metadata. | No |

## Minimum Source Set

For normal use, upload these source files:

- `agent_profile.md`
- `orchestrator_operating_model.md`
- `skill_manifest.md`
- all files in `skills/`
- all files in `templates/`

That is 17 source files. You can also upload `examples/starter_prompts.md` if you want test prompts inside the assistant context.

## Why The Files Are Organized This Way

The files are split because assistants with uploaded sources usually work better when the reference material is modular:

- `system_prompt.txt` gives the top-level behavior.
- `agent_profile.md` handles identity, tone and facilitator posture.
- `orchestrator_operating_model.md` explains the operating logic.
- `skill_manifest.md` routes the assistant to the right skill.
- `skills/` keeps each workshop block focused and easy to edit.
- `templates/` keeps final output formats separate from facilitation logic.

## Workshop Flow

1. Project brief
2. Team map
3. Assumptions and questions
4. As-is scenario map
5. Intent canvas
6. Big idea vignettes
7. Data inventory
8. Understanding map
9. Reasoning statement
10. Effects & safeguards
11. Storyboard and test plan
12. Final playback

## Note On IBM

This repository contains original prompts, skills and templates for configuring an AI facilitator. It does not include proprietary IBM materials. IBM and related framework names are trademarks of their respective owners; this project is not affiliated with or endorsed by IBM.

