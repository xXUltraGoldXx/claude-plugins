# ultragold – Claude-Code-Plugins

Marktplatz `ultragold` mit drei Plugins von Alexander (xXUltraGoldXx).

| Plugin | Inhalt | Quelle |
|---|---|---|
| `self-lern` | Skill, SessionStart-Hook und CLI `self-lern`: append-only Lerndatei, Merksätze werden beim Start geladen | [claude-self-lern](https://github.com/xXUltraGoldXx/claude-self-lern) |
| `coding-workflow` | Skill + `/cw-install`: token-effizienter Workflow (klein/mittel/groß), Planung, TODO/Analyse/Context | [coding-workflow](https://github.com/xXUltraGoldXx/coding-workflow) |
| `stil` | Skills `stil` und `projekt`: Design-Stile und Architekturen | [stil-bibliothek](https://github.com/xXUltraGoldXx/stil-bibliothek) |

## Installation

```
/plugin marketplace add xXUltraGoldXx/claude-plugins
/plugin install self-lern@ultragold
/plugin install coding-workflow@ultragold
/plugin install stil@ultragold
```

Auf der Shell: `claude plugin marketplace add xXUltraGoldXx/claude-plugins` und `claude plugin install <name>@ultragold`.

## Hinweise

- **self-lern**: Lerndatei standardmäßig `~/.claude/self-lern/LERNEN.md` (änderbar per `SELF_LERN_DATEI`). Fehlt sie, läuft der Hook ohne Fehler und meldet nur „Noch keine Eintraege“. Die CLI liegt in `bin/` des Plugins; Aufruf bei Bedarf als `python3 <Plugin-Ordner>/bin/self-lern`.
- **coding-workflow**: Einrichtung mit `/coding-workflow:cw-install` (Name, Standardgröße).
- **stil**: enthält keine Stildaten. Die Skills nutzen die öffentliche [stil-bibliothek](https://github.com/xXUltraGoldXx/stil-bibliothek) (Umgebungsvariable `STIL_BIBLIOTHEK` oder `git clone` nach `~/.claude/stil-bibliothek`, nach Rückfrage).

Lizenz: MIT, je Plugin als `LICENSE` im Plugin-Ordner (`stil` zusätzlich CC BY 4.0 für Texte der Bibliothek).

## English

Plugin marketplace `ultragold` with three plugins: `self-lern` (append-only lessons-learned file with SessionStart hook and CLI), `coding-workflow` (token-efficient development workflow skill) and `stil` (design style and architecture skills backed by the public stil-bibliothek, fetched via git clone, no style data bundled).

```
/plugin marketplace add xXUltraGoldXx/claude-plugins
/plugin install self-lern@ultragold
```

MIT licensed (see each plugin's `LICENSE`).
