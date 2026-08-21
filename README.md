# recruiting-update-template

Builds an aggregate recruiting update with funnel evidence, blockers, owners, and decisions.

It produces:

- **Weekly Recruiting Update:** a working artifact built from supplied facts, labeled inference, and visible missing fields.

It executes the [Recruiting Update Template playbook](https://www.andrewluxem.com/playbooks/recruiting-update-template). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/recruiting-update-template.git
cp -r recruiting-update-template/skills/recruiting-update-template ~/.claude/skills/
```

For Codex, copy the same complete folder to the Codex skills directory:

```bash
cp -r recruiting-update-template/skills/recruiting-update-template ~/.codex/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/recruiting-update-template
/plugin install recruiting-update-template@recruiting-update-template
```

For clients that install from an archive, use the versioned [recruiting-update-template v1.0.0 ZIP](https://www.andrewluxem.com/downloads/recruiting-update-template-v1.0.0.zip).

## Invoke it

```text
Write this week's recruiting update
Use the recruiting-update-template skill.
```

Naming the skill is always valid: `use the recruiting-update-template skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/recruiting-update-template/
  assets/weekly-recruiting-update-template.md
  LICENSE.md
  meta.yaml
  references/recruiting-update-standard.md
  SKILL.md
README.md
LICENSE
```

The complete canonical package is copied under `skills/recruiting-update-template/`, including every asset, reference, test prompt, source note, changelog entry, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, `.claude-plugin/plugin.json`, and `.claude-plugin/marketplace.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/recruiting-update-template/LICENSE.md](skills/recruiting-update-template/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.
