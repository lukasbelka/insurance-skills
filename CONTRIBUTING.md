# Contributing

Thank you for helping improve this repository.

This project is a public collection of Agent Skills: portable folders that
teach AI agents how to do specific work. Skills are meant to be installed
and used with compatible agents (CLI and desktop), including products from
Anthropic, OpenAI, Google, and others that speak the open `SKILL.md` format.

By opening a pull request, you agree that your contribution is licensed
under the **Apache License, Version 2.0**. That is the license of this
repository. Do not submit a skill unless you can offer it under those terms.

## Table of contents

- [Ways to contribute](#ways-to-contribute)
- [Before you start](#before-you-start)
- [License](#license)
- [Skill layout](#skill-layout)
- [SKILL.md frontmatter](#skillmd-frontmatter)
- [How to write a good skill](#how-to-write-a-good-skill)
- [Safety rules](#safety-rules)
- [Original work vs. third-party material](#original-work-vs-third-party-material)
- [How to test a skill](#how-to-test-a-skill)
- [Pull request process](#pull-request-process)
- [What reviewers look for](#what-reviewers-look-for)
- [What we will reject](#what-we-will-reject)
- [AI-assisted contributions](#ai-assisted-contributions)
- [Questions](#questions)

## Ways to contribute

All of the following are welcome:

| Contribution | Notes |
|---|---|
| New skill | One focused capability that is not already covered |
| Improve an existing skill | Clearer triggers, better steps, fewer tokens, working scripts |
| Fix a bug | Wrong command, stale API, broken path, misleading description |
| Docs and catalog | README, examples, installation notes |
| Validation / tooling | Checks that keep skills spec-compliant |

Small, precise changes are easier to review than large dumps.

## Before you start

1. Search the repo for an existing skill that already covers the job.
2. Search open issues and pull requests for the same idea.
3. If a skill is close, **extend that skill** instead of adding a sibling.
4. For a brand-new skill, open an issue first when the scope is large or
   ambiguous. Small, obvious additions can go straight to a PR.
5. Read the [Agent Skills specification](https://agentskills.io) and at
   least one existing skill in this repo. Copy structure, not filler.

A new skill must justify the gap in the pull request description:
what it does, when an agent should load it, and why an existing skill
is not enough.

## License

This repository is licensed under the Apache License, Version 2.0.
See the `LICENSE` file at the repository root.

### What that means for contributors

- You retain copyright in your contribution.
- You grant everyone the rights described in Apache-2.0, including
  commercial use, modification, and redistribution.
- You also grant the patent license described in Apache-2.0 for patents
  that are necessarily infringed by your contribution.
- You confirm that you have the legal right to make that grant.
- If you are contributing on behalf of an employer, you confirm that you
  are allowed to do so.

Apache-2.0 already treats a pull request as a contribution under the
same license unless you state otherwise. We do **not** accept
contributions under a different license.

### Required license field on every skill

Every `SKILL.md` **must** declare the license in YAML frontmatter:

```yaml
license: Apache-2.0