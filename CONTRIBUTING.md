# Contributing

Want to send a PR? Cool. Here's the flow.

## Before you start

- **Open an issue first** if the change is non-trivial. I don't want you to spend a weekend on something I'd have asked you to do differently.
- Read the existing files. The repository contains structured Markdown prompts, not code. Keep the style consistent.
- Look at the README to understand what this repository is about.

## Local checks

Before submitting:
- Test your game file with an actual AI model
- Check markdown formatting is correct
- Ensure all links work
- Verify token count is reasonable (single game file should not exceed 20K)

## Commit messages

I don't enforce Conventional Commits. Subject, blank line, body, done.
If a commit fixes an issue, mention the issue number. Don't bother with emoji or "WIP" prefixes.

## Pull requests

- Fill the PR template. One paragraph in the body is fine.
- Keep the diff small. Squash before merging unless the history matters.
- I'll review roughly in order of arrival. If the change does what the description says, I'll merge. I might push back on structure; that's not personal.
- Don't commit secrets, large files, or someone else's content without permission.

## What I won't merge

- Refactors that don't fix a real problem.
- Game files that haven't been tested.
- Content that violates the anti-AI-writing rules.
- Changes that break the existing structure without prior discussion.

## License

By contributing, you agree your contribution is licensed under the same license as the rest of the project. See [`LICENSE`](./LICENSE).
