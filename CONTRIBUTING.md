# Contributing

- **Branches**: `<type>/<short-description>`, e.g. `fix/broken-nav-link`, `feature/checkout-flow`.
- **Commits**: [Conventional Commits](https://www.conventionalcommits.org/) —
  `fix:`, `feat:`, `chore:`, `docs:`, `refactor:`, etc.
- **PRs required**: no direct pushes to `main`. Use the PR template.
- **Merge strategy**: squash merge only. Keep the squash commit message conventional-commit
  formatted; PR description can be longer.
- **CI is centralized**: every repo holds thin caller workflows (`.github/workflows/caller-*.yml`)
  that point at reusable workflows in
  [axiom-core-labs/acl-cicd](https://github.com/axiom-core-labs/acl-cicd). Don't add workflow
  logic in client repos — change it in `acl-cicd` instead.
- **Working with agents**: most issues in this org are written for and worked by Claude agents
  (`anthropics/claude-code-action`). Write issues to be machine-parseable — concrete objective,
  explicit scope, testable acceptance criteria. Agent-authored PRs still require human review
  before merge, same as any other PR.
