# Inspiration from Michael Kennedy's Cursor Rules

Last Updated: 28 feb 2026

````markdown
## Technical Standards

- Use Python when possible
- Use the latest Python syntax (e.g. 3.14+)
- Implement proper error handling
- Use async/await for asynchronous operations
- Prefer basic / vanilla JavaScript over frameworks.
- Run `ruff format` and `ruff check --fix` on any python files you have edited.
- Always do a git pull when starting a new chat on a project that has a git repo.
- Never put `#!/usr/bin/env python3` at the top of python scripts. We run our scripts with python out of virtual environments as `./venv/bin/python` or with `uv run`.
- Prefer `pathlib.Path` rather than `os.path` for path operations.

## Code Style

- Follow PEP8 and Ruff's formatting guidelines.
- Use guarding clauses with if + early returns rather than nested code.
- Never use `type | None` for optional types. Use `Optional[type]` instead.
- When specifying type information, please use builtin types if possible. An example is use `list[int]` over `typing.List[int]`.

## Project Structure
- Always check for a virtual environment in the workspace and activate it when running python. It may be called venv or .venv.
- Keep components, functions, etc small and focused.
- Use proper file naming conventions.
- Follow the established folder structure.
- Prefer functions in modules rather than object-oriented programming though classes are fine when they make sense.
- Prefer a stand-alone pytest.ini configuration rather than embedding these details within a pyproject.toml, even if the pyproject.toml file exists.

## Tools

- We use uv for dependency management. Use `uv pip install` rather than `pip install`
- We use uv for updating dependencies
- Please use the rules in ruff.toml for formatting if found.
- Use ruff format and ruff check for formatting and linting.
- pytest is our preferred testing framework.

## Changes

- If there is a change-log.md file in this project, it means that we wish to track changes to the project. 
- When *major* changes or features are made/added I want a concise summary of the change and files involved (summarize if too many files are changed). Use the change-log.md file to track changes and as a template.

## Config

- When running web apps for development (e.g. Flask/Quart/etc), always choose a port 10000 or higher.

At the end of every chat, please add a git commit message to help me keep the changes well desribed in git. This commit message should only summarize changes from the very last portion of our conversation - from my last request until you're finished. Do NOT commit the changes. Just show me the commit message so I can use it when I'm ready.

## Import Style Rule

**Internal project imports:**
- **Functions**: Use namespace imports (`from module import module_name` → `module_name.function()`)
- **Classes/Exceptions**: Use direct imports (`from module import TheClass`)

**Examples:**
```python
# ✅ Functions
from talkpython.services import discord_service
result = discord_service.load_discord_config()

# ✅ Classes/Exceptions  
from talkpython.services.discord_models import DiscordConfigError
raise DiscordConfigError('Error')

# ❌ Wrong
from talkpython.services.discord_service import load_discord_config
from talkpython.services import discord_models
````

