# 🧠 My Personal LLM Stack Trace

Welcome to the source code of my external cortex. This is the central registry for system prompts and AI workflows—configuration files for talking to silicon.

Objective: high availability, low latency, idempotent replies. “I dunno, I just asked a bot” is not a repeatable process.

## 📦 The Modules

Active subroutines:

- 🎓 Academic: Rigorous assessment logic (see [Academic/IELTS-Writing/IELTS-Writing.md](Academic/IELTS-Writing/IELTS-Writing.md)). Less hallucination, more red pen.
- ☕ Daily Life: Coming soon—algorithms for adulting, meal prep, and other IRL DLCs.
- 💻 Software Development: Coming soon—pair programmers that never hog the keyboard.

## 🗺️ File System Architecture

- [Academic/](Academic/): Specialized agents useful for academic purposes.
- [.github/README.md](.github/README.md): You are here (0x00). The documentation root.
- [.github/TODO.md](.github/TODO.md): The backlog—where features go to dream (or deprecate).

## ⚙️ Runtime Instructions (Usage)

To deploy these prompts into your preferred LLM runtime environment:

1. Inject the payload: copy the system prompt. Don’t amputate Role or Guardrails unless you enjoy undefined behavior.
2. Pass arguments: swap placeholders for your real context (task, constraints, output format).
3. Unit test: for evaluations, paste your draft first. No pre-baked essays; we optimize for learning, not plagiarism.
4. Commit the diff: if you improve a prompt mid-chat, upstream it so Git can remember.

## 📏 Linting Rules (Conventions)

When pushing new prompts to main, adhere to these coding standards:

- Initialization: define Role, Mission, Tone, Audience.
- Exception handling: add Guardrails; ban bad behaviors explicitly.
- Data types: bullets beat rambling prose.
- Encoding: ASCII unless the task demands flair.
- Rubrics: if criteria exist, name them—don’t let the AI invent weights.

## 🧬 The Boilerplate (Template)

Copy this class definition when initializing a new prompt instance:

```markdown
# <Prompt Name>

## Role
- <The Entity's Persona>
- Mission parameters (e.g., "Be harsh but fair")

## Audience
- <User Profile / Difficulty Level>

## Guardrails (Exceptions)
- <Forbidden operations>
- <Halt conditions>

## Workflow (Logic Flow)
1) <Input processing>
2) <Logic execution>
3) <Output rendering>

## Output Schema
- <JSON-like structure or specific headers required in response>

## Dependencies
- <Rubrics, vocabulary lists, external references>

```

## 🧹 Garbage Collection & Refactoring

- Atomic commits: small edits. Five-thousand-token diffs are review kryptonite.
- Regression testing: run a “Hello World” chat before pushing.
- Logs: if a prompt fails, note the failure mode in the file or commit; don’t reintroduce the same bug.

## 🔮 Roadmap

See [.github/TODO.md](.github/TODO.md) for the backlog and patch notes.

## 🛠️ Contribution Guidelines

Feel free to fork and submit pull requests. See [.github/CONTRIBUTING.md](.github/CONTRIBUTING.md). Follow the linting rules and include sample conversations as “unit tests” for major changes.
