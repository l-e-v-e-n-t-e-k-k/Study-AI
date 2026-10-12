# Study AI

**Learn actively, not just by reading answers.**

Study AI is a collection of learning skills for Codex that turns an AI assistant into an adaptable study partner. Whether you are exploring a new subject, trying to understand a difficult idea, preparing for a test, or reviewing your own work, Study AI helps you focus on the next useful learning step.

It works across subjects—from mathematics and science to languages, economics, and programming. You can describe what you need in everyday language; you do not have to choose a skill yourself.

## Key Features

- **Adaptive learning:** Tailors questions, examples, and difficulty to your goal and demonstrated understanding.
- **Understanding over memorization:** Explores intuition, underlying mechanisms, and practical applications.
- **Active participation:** Encourages independent reasoning, recall, and problem-solving instead of passive reading.
- **Evidence-based feedback:** Distinguishes demonstrated understanding from assumptions and identifies actionable gaps.
- **Focused interactions:** Keeps responses organized and as concise as the learning task allows, without sacrificing necessary depth.

## Learning Roles

| Skill | What it helps you do |
| --- | --- |
| **Interviewer** | Clarify your learning goal, assess relevant prior knowledge, and identify where to begin. |
| **Explainer** | Understand concepts and overcome specific obstacles with clear mechanisms and worked examples. |
| **Socratic Questioner** | Challenge your reasoning through adaptive questions and progressively useful hints. |
| **Examiner** | Test independently demonstrated knowledge with questions that adapt to your performance. |
| **Checker** | Review your solutions and reasoning, identify errors, and suggest improvements without taking over your work. |

## Installation

### Option A — Codex Plugin (Recommended)

Install **Study AI** from a Codex plugin marketplace that distributes it:

1. Open Codex and access the plugin browser
2. Select the marketplace containing **Study AI**, then choose the plugin and install it.
3. Start a new conversation and describe what you want to learn.

If you need to register a marketplace source first, follow the [Codex plugin marketplace instructions](https://developers.openai.com/plugins/build/plugins). A plugin marketplace must include Study AI before it can be installed from that source.

### Option B — Manual Skill Installation

Download or clone this repository. From its root, copy the folders inside `skills/` into a Codex skill location:

- **Personal:** `~/.agents/skills/` — available across your projects.
- **Project:** `<your-project>/.agents/skills/` — available within that project.

For macOS or Linux, to install all skills personally:

```bash
mkdir -p ~/.agents/skills
cp -R skills/. ~/.agents/skills/
```

On Windows, copy the five folders from `skills/` to `%USERPROFILE%\.agents\skills\`, or to the `.agents\skills\` folder of your chosen project.

Start a new Codex conversation after installation. Neither installation method requires editing your personal `AGENTS.md`.

## Getting Started

Try any of these prompts:

| Goal | Example prompt |
| --- | --- |
| Find a starting point | “I want to learn economics, but I'm not sure where to begin.” |
| Understand a concept | “Explain how neural networks learn, starting with the intuition.” |
| Think more deeply | “I think I understand probability. Challenge me with questions.” |
| Test yourself | “Quiz me on human biology, one question at a time.” |
| Review your work | “Check my mathematical proof and point out mistakes without rewriting it.” |

You can also request a role explicitly, such as: “Use the Socratic Questioner to help me understand recursion.”

## How It Works

Codex selects a relevant learning skill from your request and the available conversation context. One role guides the current activity, while small supporting techniques may be used when helpful. When a substantially different learning mode would be useful, Study AI proposes the change rather than abruptly switching modes; your explicit request can initiate a switch directly.

Each role has its own approach to pacing, feedback, and completion. Relevant context—such as your goal, previous answers, and observed uncertainties—can be reused within the available conversation. Skill selection and transitions are model-guided rather than a rigid, scripted sequence.

## Learning Philosophy

Study AI follows four simple principles:

- **Understand why:** Build mental models and connect ideas to first principles.
- **Practice independently:** Demonstrate what you can do without relying on assisted solutions.
- **Learn from evidence:** Use your responses and work to identify the next useful step.
- **Avoid overload:** Prefer targeted questions, clear structure, and necessary depth over long, repetitive explanations.

**You decide what to learn. Study AI helps you learn it deliberately.**
