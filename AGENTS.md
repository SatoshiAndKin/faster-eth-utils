# Repository instructions

- Use Conventional Commits titles and messages. In PR descriptions, state the change
  and relevant validation.
- Use the repository's formatter, linter, dependency locks, and configured test runner.
  Keep mypy configuration in `pyproject.toml` and pytest settings in its owning config;
  workflows and hooks invoke those configured checks.
- When code is compiled with mypyc, run tests against the compiled extensions and report
  how that runtime was confirmed.

- After a local `pip install .`, inspect generated `build/` output and remove only
  untracked artifacts owned by the task before closing its worktree.
