# Kaptain Marketplace

Browse and install plugins for the [Kaptain](https://github.com/kube-kaptain) general purpose build and Kubernetes deploy system.


## Available Plugins

| Plugin | Description |
|--------|-------------|
| [kaptain-skills](https://github.com/kube-kaptain/kaptain-skills) | Skills for the Kaptain general purpose build and Kubernetes deploy system |


## Installation

Installation varies by your choice of LLM, see below for whichever you're using.

### Claude Code

```bash
claude plugin add kaptain-skills@kaptain-marketplace
```

### Cursor

```
/add-plugin kaptain-skills
```

### Codex

See [kaptain-skills/.codex/INSTALL.md](https://github.com/kube-kaptain/kaptain-skills/blob/main/.codex/INSTALL.md)

### Gemini CLI

```bash
gemini extensions install https://github.com/kube-kaptain/kaptain-skills
```

### OpenCode

Add to `opencode.json`:

```json
{
  "plugin": ["kaptain-skills@git+https://github.com/kube-kaptain/kaptain-skills.git"]
}
```
