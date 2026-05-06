# AGENTS.md

Static HTML/CSS CV site. No build system, no tests, no package manager.

## Git practices

- Never commit without explicit user request
- Keep commit messages concise (1-2 sentences, focus on why not what)
- Do not commit `preferences.json` (local user config)

## Push workflow

Git push requires `gh` CLI authentication. Use:
```
GITHUB_TOKEN=$(gh auth token) && git push https://jimenaluperdi-es:${GITHUB_TOKEN}@github.com/jimenaluperdi-es/webcv.git master
```
## Git
- Commit only when explicitly requested by the user
- Commit messages: concise, present tense, describe the exact change (e.g., "Update name to Jimena Luperddi")
- Never force push to main; warn user if requested
- Push to remote only when explicitly asked

- Commit Types:
Type     Purpose
feat     New feature
fix     Bug fix
docs     Documentation only
style     Formatting/style (no logic)
refactor     Code refactor (no feature/fix)
perf     Performance improvement
test     Add/update tests
build     Build system/dependencies
ci     CI/config changes
chore     Maintenance/misc
revert     Revert commit
- Generate Commit Message
    Type: What kind of change is this?
    Scope: What area/module is affected?
    Description: One-line summary of what changed (present tense, imperative mood, <72 chars)

- Execute Commit

# Single line
git commit -m "<type>[scope]: <description>"
git commit -m "<feat>[language]: <add italiano basic language>
