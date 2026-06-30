# Source File Checklist

Use this checklist when setting up the assistant in ChatGPT, Gemini or Claude.

## Copy Into Instructions

Copy the full content of this file into the assistant/project/gem instructions:

- `system_prompt.txt`

Do not upload `system_prompt.txt` as a source unless your platform requires all instructions to be uploaded as files.

## Core Sources To Upload

Upload these 17 source files:

1. `agent_profile.md`
2. `orchestrator_operating_model.md`
3. `skill_manifest.md`
4. `skills/01_workshop_intake.md`
5. `skills/02_team_and_assumptions.md`
6. `skills/03_scenario_mapping.md`
7. `skills/04_ai_intent_design.md`
8. `skills/05_big_idea_generation.md`
9. `skills/06_data_inventory.md`
10. `skills/07_understanding_reasoning.md`
11. `skills/08_effects_safeguards.md`
12. `skills/09_storyboard_test_plan.md`
13. `skills/10_playback_pdf_delivery.md`
14. `skills/11_relational_trust_language_adaptation.md`
15. `templates/canvas_state_schema.md`
16. `templates/final_workbook_template.md`
17. `templates/html_pdf_template.md`

## Optional Source

Upload this only if you want starter examples available inside the assistant:

- `examples/starter_prompts.md`

## Do Not Upload As Assistant Sources

These files are for humans or for GitHub:

- `README.md`
- `source_file_checklist.md`
- `.gitignore`
- `LICENSE`

## Platform Notes

- ChatGPT: use Project Instructions or Custom GPT Instructions, then upload the core sources as knowledge.
- Gemini: use Gem instructions, then upload the core sources if file knowledge is available.
- Claude: use Project instructions, then upload the core sources as project knowledge.

If the platform supports file generation or code execution, enable it so the assistant can create printable HTML/PDF outputs.

