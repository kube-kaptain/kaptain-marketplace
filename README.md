# Kaptain Marketplace

Browse and install plugins for the [Kaptain](https://github.com/kube-kaptain) general purpose build and Kubernetes deploy system.


## Available Plugins

| Plugin | Description |
|--------|-------------|
| [kaptain-skills](https://github.com/kube-kaptain/kaptain-skills) | Skills for the Kaptain general purpose build and Kubernetes deploy system |


## Installation

Installation varies by LLM coding agent.

### Claude Code

Register this marketplace, then install the skills:

```bash
/plugin marketplace add kube-kaptain/kaptain-marketplace
/plugin install kaptain-skills@kaptain-marketplace
```

Or from the terminal:

```bash
claude plugin marketplace add kube-kaptain/kaptain-marketplace
claude plugin install kaptain-skills@kaptain-marketplace
```

### Cursor

In the Cursor IDE, go to **Dashboard > Settings > Plugins > Import** and paste:

```
https://github.com/kube-kaptain/kaptain-marketplace
```

Browse the imported marketplace and install `kaptain-skills` from the plugin panel.

### Codex

Clone the skills repo and symlink it into the Codex skills directory:

```bash
git clone https://github.com/kube-kaptain/kaptain-skills.git ~/.codex/kaptain-skills
mkdir -p ~/.agents/skills
ln -s ~/.codex/kaptain-skills/skills ~/.agents/skills/kaptain-skills
```

### Gemini CLI

Install the skills repo as an extension:

```
/extensions install https://github.com/kube-kaptain/kaptain-skills
```

Or from the terminal:

```bash
gemini extensions install https://github.com/kube-kaptain/kaptain-skills
```

### OpenCode

Add to the `plugin` array in your project's `opencode.json`:

```json
{
  "plugin": ["kaptain-skills@git+https://github.com/kube-kaptain/kaptain-skills.git"]
}
```


## License

MIT
