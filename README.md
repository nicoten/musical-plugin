# Musical

An interactive music theory teacher and practice coach, packaged as a plugin for
Claude and ChatGPT.

It drills chords, intervals, scales and modes, key signatures, rhythm and
notation. It practises by default rather than lecturing, grades answers strictly
(including spelling - G# and Ab are different answers), starts at beginner level
and adapts upward, and always replies in the learner's own language.

It needs no network access, no connectors and no external services.

## Install

### Claude Code

```
/plugin marketplace add nicoten/musical-plugin
/plugin install musical@nicoten
```

### Claude Cowork, and claude.ai

Open **Customize -> Plugins**, select **Add marketplace**, and enter
`nicoten/musical-plugin`. Then select Musical and click **Install**.

Plugins are read by Cowork and Claude Code. They are not read by claude.ai
**Chat** - upload the standalone skill there instead, from
<https://musical.nicotejera.com/ai/skill.zip>.

### ChatGPT, and Codex

Musical is in the ChatGPT plugin directory:

<https://chatgpt.com/plugins/plugins_6aaf0c4ee1648191840a709e424ebb41>

That covers ChatGPT on the web, mobile and the desktop app, and Codex. Invoke it
with `@musical` in ChatGPT, or `$musical` in Codex. It also triggers on its own
when a request matches music theory practice.

To run an unreleased version, clone this repository instead: its
`.agents/plugins/marketplace.json` makes the checkout a local marketplace.

```bash
git clone https://github.com/nicoten/musical-plugin.git
```

For anywhere that takes an uploaded plugin folder rather than a marketplace,
the plugin is downloadable as an archive: <https://musical.nicotejera.com/ai/plugin.zip>

## Companion app

<https://musical.nicotejera.com> - staff notation and audio for the exercises
that are better heard than read. Optional; the plugin is complete without it.

## Source

This repository is generated. The skill is developed in the app's repository and
published from there, so edits made here would be overwritten on the next
release. Issues and suggestions are welcome.

MIT licensed.
