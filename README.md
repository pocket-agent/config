# config

Workspace configuration for the [Pocket Agent](https://github.com/pocket-agent) ecosystem.

**GitHub:** [pocket-agent/config](https://github.com/pocket-agent/config)

## Contents

| File | Purpose |
|------|---------|
| `modules.yaml` | Module install registry (`pocket-agent init` / wizard) |
| `setup.defaults.yaml` | Defaults copied to `user-setup.yaml` on first setup |
| `user-setup.yaml` | Local connection profile (not committed — see `.gitignore`) |

## Bootstrap (new machine)

Clone this repo **first** into the workspace `config/` folder, then sibling repos:

```bash
mkdir -p ~/pocket-agent && cd ~/pocket-agent
git clone https://github.com/pocket-agent/config.git config
git clone https://github.com/pocket-agent/scripts.git scripts
git clone https://github.com/pocket-agent/pocket-agent.git pocket-agent
./scripts/setup-local.sh
```

## Docs

Workspace layout and profiles are documented in the agent monorepo workspace (`docs/WORKSPACE_LAYOUT.md`, `docs/API_STACK.md`) when you use the full org folder in Cursor.
