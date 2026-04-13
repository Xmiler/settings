# Global preferences

## Language
- Respond in Russian
- Code, comments, variable names, docstrings — in English
- Commit messages — in English

## Code style
- Python 3.10+
- Type hints only for public functions
- Use venv/pip for environments
- Bash scripts where needed
- Keep code simple and readable — no over-engineering

## Preferred libraries
- pathlib for all file/path operations (not os.path)
- click for CLI interfaces
- tqdm for progress bars
- tabulate for table output
- joblib for parallelism and caching

## Behavior
- Before large changes (3+ files or major refactoring): outline the plan and wait for approval
- Do not run scripts (python, bash) without my confirmation
- Do not commit to git automatically — suggest a commit message and wait
- When the task is simple — just do it, no need to ask

## Response style
- Adapt verbosity to the task: short answers for simple questions, detailed for complex ones
- No unnecessary preambles like "Great question!" — get to the point
- When suggesting code changes, show only the relevant diff, not the entire file
- If something is unclear — ask, don't guess

## Git
- Commit messages in English, lowercase, imperative mood
- Format: `type: description` (e.g. `fix: handle empty response from model`)
- Keep commits atomic — one change per commit
