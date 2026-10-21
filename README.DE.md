# Spec Kit (Deutsch · Java-Ausrichtung)

**Fork von [github/spec-kit](https://github.com/github/spec-kit)** — übersetzt ins Deutsche und angepasst für **Java-Projekte**, erweitert um Prompting-, Scrum- und Kanban-Wissen sowie die **OpenClaw-Verhaltensregeln**.

> This repository is a German-language, Java-oriented fork of GitHub's Spec Kit. Dokumentation und Templates sind auf Deutsch; die technischen Beispiele und Projektstrukturen sind auf das Java-Ökosystem (Maven/Gradle, JUnit 5, Spring Boot) ausgerichtet.

## Was ist das?

Spec Kit ist ein Toolkit für **spec-driven development (SDD)** — du beschreibst Features in natürlicher Sprache, und ein Agent generiert daraus Spezifikation, Implementierungsplan, Aufgabenliste und Checklisten.

## Was ist anders als im Original?

1. **Deutsch**: Templates (`spec`, `constitution`, `plan`, `tasks`, `checklist`) und Command-Definitionen auf Deutsch.
2. **Java-Ausrichtung**: Beispiel-Strukturen, Pfad-Konventionen (`src/main/java/`, `src/test/java/`), Testbeispiele (JUnit 5) und Build-Werkzeuge (Maven/Gradle) angepasst.
3. **Agiles Wissen integriert**: Kernprinzipien aus *Scrum kurz & gut*, *Kanban* (Anderson/Bartel) und *Prompting kurz & gut* fließen in die Arbeitsweise ein (WIP-Limits, Definition of Done, Iterativer Prompt-Aufbau).
4. **Verhaltensregeln**: Die **OpenClaw-Regeln** (Wahrhaftigkeit & Güte — epistemische Integrität nach Meredith Whittaker + buddhistische Ethik) sind als Leitplanken eingebunden.

## Schnellstart

1. Klone dieses Repository.
2. Nutze die Templates unter `templates/` als Ausgangspunkt für deine Specs.
3. Wähle das deutsche Template (`-de.md`) für deine Feature-Spezifikationen.

## Struktur

- `templates/` — Vorlagen (deutsch `-de.md` und englisch original)
- `templates/commands/` — Command-Definitionen für die SDD-Workflows
- `docs/` — Dokumentation

## Lizenz

Wie das Original: siehe `LICENSE`.
