# Coding practices

- Always run the project's configured linter after writing or changing code and before handing off the work. Use the repository's documented commands and configuration. Fix lint errors introduced by your changes; report unrelated existing failures. If no linter is configured or linting cannot run, explicitly say so and explain why. Do not claim lint passed without running it, and do not add or change lint tooling without task justification.
- Read applicable repository instructions and nearby code before editing. Follow established architecture, naming, formatting, and dependency conventions.
- Make the smallest coherent change that solves the requested problem. Avoid unrelated refactors, speculative abstractions, and unnecessary dependencies.
- Prefer clear, maintainable code with descriptive names and straightforward control flow. Add comments to explain non-obvious intent or constraints, rather than restating the code.
- Validate inputs at trust boundaries, handle expected errors explicitly, and avoid silently swallowing failures. Never commit secrets or expose sensitive data in logs or error messages.
- Preserve existing user changes. Avoid destructive commands, broad rewrites, and changes outside the requested scope.
- Add or update meaningful tests for behavior changes and bug fixes when appropriate. Run relevant tests, formatting checks, type checks, and builds proportionate to the change and any repository requirements.
- Preserve public interfaces and backward compatibility unless the task calls for a change. Update affected documentation and examples when behavior, configuration, or usage changes.
- Review the final diff for accidental edits, debug code, unused code, and sensitive data. Keep generated files and lockfiles consistent when applicable.
- Follow Conventional Commits for commit messages: use `<type>[optional scope][!]: <description>` (for example, `feat(auth): add password reset`). Use `feat` for new features, `fix` for bug fixes, and other appropriate types such as `docs`, `refactor`, `test`, or `chore`. Mark breaking changes with `!` before the colon or a `BREAKING CHANGE:` footer.
- In the handoff, briefly explain what changed, which checks actually ran and their results, and any remaining limitations or blockers.
