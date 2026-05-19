# AGENTS.md

## Cursor Cloud specific instructions

This is currently an empty/placeholder repository with only a `README.md` file. There is no application code, no dependencies, no build system, and no services to run.

### Available tools in the VM

- Node.js v22 (via nvm)
- Python 3.12
- Git 2.43

### Notes for future agents

- When application code is added, update the update script via `SetupVmEnvironment` to install the relevant dependencies.
- There are no lint, test, or build commands available until source code is added.
- No `.env` files or secrets are required at this time.
