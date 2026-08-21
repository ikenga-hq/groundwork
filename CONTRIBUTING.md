# Contributing to groundwork

Thanks for helping make groundwork better. It's an open Claude Code skill (Apache-2.0).

## This is the canonical home

`ikenga-hq/groundwork` is the source of truth for the skill and the `npx skills add ikenga-hq/groundwork` install surface. Edit the skill under `skills/groundwork/`, open a PR here, and CI will check that `SKILL.md` still resolves for `npx skills`.

> **Transitional note:** groundwork is also published to npm as `@ikenga/skill-groundwork` from the [`ikenga-pkgs`](https://github.com/ikenga-hq/ikenga-pkgs) monorepo. The sync that keeps the two in step is being reversed so this repo is fully canonical (the publish pipeline will consume from here). Until that lands, a maintainer mirrors merged changes into `ikenga-pkgs` for the npm release — your PR here is still the place to make changes.

## Making a change

1. Fork + branch.
2. Edit `skills/groundwork/` (the skill: `SKILL.md`, `actions/`, `agents/`, `lib/`, `profiles/`, `scripts/`).
3. Keep `SKILL.md` frontmatter (`name` + `description`) intact — CI validates it.
4. Don't change the install path (`ikenga-hq/groundwork`) or the published npm name (`@ikenga/skill-groundwork`) — they're hard invariants.
5. Update the README / [docs](https://ikenga.dev/docs/groundwork) if you change behaviour or actions.
6. Open a PR; fill in the template.

## Trying it locally

```bash
npx skills add ikenga-hq/groundwork    # project install
# or from a clone:
git clone https://github.com/ikenga-hq/groundwork.git
```

## License

By contributing you agree your contributions are licensed under [Apache-2.0](LICENSE).
