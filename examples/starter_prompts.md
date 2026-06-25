# Starter prompts

## Simple start

```text
/start
```

## Start with context

```text
Guide me through the AI Solutions Canvas workshop.

Context: we want to understand whether it makes sense to use AI to help customer support find answers faster.
Users: support agents and end customers.
Constraints: data in Zendesk tickets, knowledge base not always up to date, attention to privacy and answer quality.
```

## Test del facilitatore

```text
I already have an idea: I want to build an AI chatbot for customers. Guide me through the canvas and tell me whether it is actually a good idea.
```

Expected behavior:

- The GPT must not accept "chatbot" as the solution too quickly.
- It must return to user, current situation, problem and outcome.
- It must then move through data, understanding, reasoning and safeguards.

## PDF request

```text
/pdf
```

Expected behavior:

- If the canvas is incomplete, the GPT asks the missing questions.
- If the canvas is complete, it produces playback, workbook, HTML and PDF.
