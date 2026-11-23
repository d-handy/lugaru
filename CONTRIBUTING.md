# Contributing

## Workflow

1. Open an issue first, using one of the issue templates.
2. Create a branch from the current `master`:
   `<type>/<issue-number>-<short-description>`, e.g. `fix/42-uninitialized-yaw`.
3. Write commit messages following [Conventional Commits](https://www.conventionalcommits.org/):

   ```
   fix: initialize player yaw before use

   The level loader read playerYaw before it was set.

   Closes #42
   ```

   - Types: `feat`, `fix`, `refactor`, `perf`, `test`, `build`, `ci`, `docs`, `chore`
   - Summary in lowercase and imperative mood, no trailing period
   - The body explains why the change is needed
   - `Closes #<nr>` only in the commit that resolves the issue, otherwise `Refs #<nr>`
4. Keep one logical change per commit.

## Building

See the [README](README.md) and [COMPILING.md](COMPILING.md).
Before opening a pull request, build from a fresh build directory and
make sure no new compiler warnings appear.

## Pull requests

- Reference the issue in the description (`Closes #<nr>`).
- The CI build must pass; `master` is protected and only accepts
  pull requests with a green build.
- Pull requests are squash-merged, so the commit messages become the
  documentation in the history.