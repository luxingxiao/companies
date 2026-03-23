# RedOak Review

> A boutique code quality, design, and security review agency powered by pragmatic, opinionated review workflows.

Built from [Patrick Ellis's Claude Code Workflows](https://github.com/OneRedOak/claude-code-workflows), which provides structured review methodologies for code quality, UI/UX design, and security analysis.

## How it works

The **CEO / Lead Reviewer** receives review requests and dispatches to the appropriate specialist. Work flows through the organization in a hub-and-spoke model:

```
         +--------- CEO / Lead Reviewer ---------+
         |              |              |           |
   Code Reviewer  Design Reviewer  Security   CI Integration
                                   Reviewer     Engineer
```

| Review Type | Specialist | Methodology |
|-------------|-----------|-------------|
| Code Quality | Code Reviewer | 7-tier pragmatic hierarchy: Architecture > Functionality > Security > Maintainability > Testing > Performance > Dependencies |
| UI/UX Design | Design Reviewer | 8-phase live-browser review at 1440px, 768px, 375px viewports |
| Security | Security Reviewer | 3-phase analysis with >80% confidence threshold and false-positive filtering |
| CI/CD | CI Integration Engineer | GitHub Actions pipelines for all three review types |

## What's Inside

> This is an [Agent Company](https://agentcompanies.io) package from [Paperclip](https://paperclip.ing)

| Content | Count |
|---------|-------|
| Agents | 5 |
| Skills | 6 |

### Agents

| Agent | Title | Reports To | Skills |
|-------|-------|------------|--------|
| **CEO** | CEO / Lead Reviewer | -- | -- |
| Code Reviewer | Senior Code Reviewer | ceo | pragmatic-code-review |
| Design Reviewer | Senior Design Reviewer | ceo | design-review |
| Security Reviewer | Senior Security Reviewer | ceo | security-review |
| CI Integration Engineer | CI/CD Integration Engineer | ceo | code-review-action, design-review-action, security-review-action |

### Skills

| Skill | Description | Source |
|-------|-------------|--------|
| pragmatic-code-review | 7-tier hierarchical code quality review with triage levels | [github](https://github.com/OneRedOak/claude-code-workflows/blob/main/code-review/pragmatic-code-review-subagent.md) |
| design-review | 8-phase UI/UX design review across three viewports | [github](https://github.com/OneRedOak/claude-code-workflows/blob/main/design-review/design-review-agent.md) |
| security-review | 3-phase security review with confidence scoring | [github](https://github.com/OneRedOak/claude-code-workflows/blob/main/security-review/security-review-slash-command.md) |
| code-review-action | GitHub Actions workflow for automated code review | [github](https://github.com/OneRedOak/claude-code-workflows/blob/main/code-review/claude-code-review-custom.yml) |
| design-review-action | GitHub Actions integration for automated design review | [github](https://github.com/OneRedOak/claude-code-workflows/blob/main/design-review/design-review-slash-command.md) |
| security-review-action | GitHub Actions workflow for automated security review | [github](https://github.com/OneRedOak/claude-code-workflows/blob/main/security-review/security.yml) |

## Getting Started

```bash
pnpm paperclipai company import this-github-url-or-folder
```

See [Paperclip](https://paperclip.ing) for more information.

## References

- **Source repo**: [OneRedOak/claude-code-workflows](https://github.com/OneRedOak/claude-code-workflows) — Code review, design review, and security review workflows by Patrick Ellis
- **Agent Companies spec**: [agentcompanies.io/specification](https://agentcompanies.io/specification)
- **Paperclip**: [github.com/paperclipai/paperclip](https://github.com/paperclipai/paperclip)

## License

MIT -- see [LICENSE](LICENSE)
