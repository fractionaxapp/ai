# fractionaxapp/ai

The **AI tier** of the [FractionAX](https://github.com/fractionaxapp/fractionaxapp)
meta-monorepo. This repo is an umbrella that groups the AI/ML services, each wired
in as its own git submodule:

| Submodule | Repo | What it is |
| --- | --- | --- |
| `agents/` | [`fractionaxapp/agents`](https://github.com/fractionaxapp/agents) | Claude tool-use agents service (FastAPI) |

> This repo is itself a submodule of the
> [`fractionaxapp`](https://github.com/fractionaxapp/fractionaxapp) meta-monorepo,
> mounted at `ai/`. So the agents service lives at `ai/agents` in the meta-repo.
> Develop from the meta-repo, where moon orchestrates every project.

## Clone

```bash
git clone --recurse-submodules https://github.com/fractionaxapp/ai.git
```

Add a new AI service here with `git submodule add <url> <name>`, then commit the
pointer.
