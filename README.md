# IBM AI Solutions ChatGPT Facilitator

Repository per configurare un progetto ChatGPT che faciliti un workshop AI Solutions Canvas ispirato a pratiche di AI human-centered design, Enterprise Design Thinking e AI Essentials.

L'obiettivo del progetto e aiutare un gruppo con competenze AI anche molto diverse a passare da un problema reale a una proposta AI ragionata, verificabile e responsabile.

## Language behavior

The default language is English. At the beginning of every new workshop, the agent must first ask, in English:

```text
Which language would you like to use for this workshop? You can answer in any language.
```

After that, the agent continues in the language chosen by the user. If the answer is absent or ambiguous, it continues in English.

## Cosa fa l'agente

- Guida un percorso unico, senza varianti di test.
- Fa poche domande alla volta.
- Compila progressivamente un AI Solutions Canvas.
- Tiene conto della dimensione relazionale: scetticismo, linguaggio non tecnico, fiducia, timore di sostituzione, controllo umano.
- Produce playback finale, decisione e workbook.
- Se ChatGPT lo consente, genera anche HTML/PDF stampabile.

## Struttura

```text
.
├── system_prompt.txt
├── agent_profile.md
├── orchestrator_operating_model.md
├── skill_manifest.md
├── source_file_checklist.md
├── skills/
│   ├── 01_workshop_intake.md
│   ├── 02_team_and_assumptions.md
│   ├── 03_scenario_mapping.md
│   ├── 04_ai_intent_design.md
│   ├── 05_big_idea_generation.md
│   ├── 06_data_inventory.md
│   ├── 07_understanding_reasoning.md
│   ├── 08_effects_safeguards.md
│   ├── 09_storyboard_test_plan.md
│   ├── 10_playback_pdf_delivery.md
│   └── 11_relational_trust_language_adaptation.md
├── templates/
│   ├── canvas_state_schema.md
│   ├── final_workbook_template.md
│   └── html_pdf_template.md
└── examples/
    └── starter_prompts.md
```

## Setup in ChatGPT

1. Crea un nuovo Project in ChatGPT.
2. Copia il contenuto di `system_prompt.txt` nelle istruzioni del Project.
3. Carica come knowledge i file indicati in `source_file_checklist.md`.
4. Se disponibile, abilita strumenti di analisi dati / creazione file.
5. Start with:

```text
/start
```

Or:

```text
Guide me through the AI Solutions Canvas workshop.
```

## Limite fonti

Il progetto e pensato per stare sotto il limite di 25 fonti.

- Fonti da caricare in ChatGPT: 19.
- `system_prompt.txt`: da copiare nelle istruzioni, non serve caricarlo come fonte.
- `source_file_checklist.md`: file di servizio, opzionale.

## Flusso workshop

1. Project brief
2. Team map
3. Assunzioni e domande
4. As-is scenario map
5. Intent canvas
6. Big idea vignettes
7. Data inventory
8. Understanding map
9. Reasoning statement
10. Effects & safeguards
11. Storyboard e test plan
12. Playback finale

## Decisione finale

L'agente chiude sempre con una delle quattro decisioni:

- Go
- Pivot
- Research first
- Stop

## Nota su IBM

Questo repository contiene prompt, skill e template originali per configurare un facilitatore ChatGPT. Non include materiali proprietari IBM. IBM e i nomi dei relativi framework sono marchi dei rispettivi proprietari; questo progetto non e affiliato o approvato da IBM.
