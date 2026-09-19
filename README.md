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

### ChatGPT desktop, and Codex

Clone this repository somewhere permanent. Its
`.agents/plugins/marketplace.json` makes it a local marketplace:

```bash
git clone https://github.com/nicoten/musical-plugin.git
```

Then restart the ChatGPT desktop app. Invoke it with `@musical` in ChatGPT, or
`$musical` in Codex. It also triggers on its own when a request matches music
theory practice.

## Companion app

<https://musical.nicotejera.com> - staff notation and audio for the exercises
that are better heard than read. Optional; the plugin is complete without it.

## Source

This repository is generated. The skill is developed in the app's repository and
published from there, so edits made here would be overwritten on the next
release. Issues and suggestions are welcome.

MIT licensed.
