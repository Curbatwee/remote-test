# AGENTS.md

## Project overview

This repository (`remote-test`) is a minimal placeholder/test repo. It contains only two text files:

- `a.txt` — content: `aaaaaaaa`
- `test.txt` — content: `test`

There is no application source code, package manager, build system, or test suite.

## Cursor Cloud specific instructions

### Services

No services need to be started. There is no frontend, backend, database, or Docker Compose stack.

### Lint / test / build / run

None of these apply — there are no configured lint, test, build, or dev-server commands.

To verify the repo is intact, run:

```bash
test "$(cat a.txt)" = "aaaaaaaa" && test "$(cat test.txt)" = "test" && echo "OK"
```

### Gotchas

- This repo has no `README.md`, `package.json`, or other setup files. Do not expect `npm install`, `pip install`, or similar steps.
- If you were sent here expecting a full application, confirm the correct repository/branch is checked out.
