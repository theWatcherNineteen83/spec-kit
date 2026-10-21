---
description: "Aufgabenlisten-Vorlage für die Feature-Implementierung"
---

# Aufgaben: [FEATURE-NAME]

**Eingabe**: Designdokumente aus `/specs/[###-feature-name]/`

**Voraussetzungen**: plan.md (erforderlich), spec.md (erforderlich für User Stories), research.md, data-model.md, contracts/

**Tests**: Die Beispiele unten enthalten Testaufgaben. Tests sind OPTIONAL – nur einbeziehen, wenn explizit in der Feature-Spezifikation gefordert.

**Organisation**: Aufgaben sind nach User Story gruppiert, damit jede Story unabhängig implementiert und getestet werden kann.

## Format: `[ID] [P?] [Story] Beschreibung`

- **[P]**: Kann parallel laufen (verschiedene Dateien, keine Abhängigkeiten)
- **[Story]**: Zu welcher User Story diese Aufgabe gehört (z.B. US1, US2, US3)
- Exakte Dateipfade in Beschreibungen angeben

## Pfad-Konventionen

- **Einzelprojekt**: `src/main/java/`, `src/test/java/` in der Repository-Wurzel
- **Web-App**: `backend/src/main/java/`, `frontend/src/`
- Pfade unten gehen vom Einzelprojekt aus – an Struktur aus plan.md anpassen

<!--
  ============================================================================
  WICHTIG: Die Aufgaben unten sind BEISPIELAUFGABEN nur zur Veranschaulichung.

  Der Befehl __SPECKIT_COMMAND_TASKS__ MUSS diese durch echte Aufgaben ersetzen, basierend auf:
  - User Stories aus spec.md (mit Prioritäten P1, P2, P3...)
  - Feature-Anforderungen aus plan.md
  - Entitäten aus data-model.md
  - Endpunkte aus contracts/

  Aufgaben MÜSSEN nach User Story organisiert sein, damit jede Story:
  - unabhängig implementiert
  - unabhängig getestet
  - als MVP-Inkrement geliefert werden kann

  Diese Beispielaufgaben NICHT in der generierten tasks.md behalten.
  ============================================================================
-->

## Phase 1: Einrichtung (gemeinsame Infrastruktur)

**Zweck**: Projektinitialisierung und Grundstruktur

- [ ] T001 Projektstruktur gemäß Implementierungsplan anlegen
- [ ] T002 [Sprache]-Projekt mit [Framework]-Abhängigkeiten initialisieren (Maven/Gradle)
- [ ] T003 [P] Linting und Formatierung konfigurieren

---

## Phase 2: Grundlagen (blockierende Voraussetzungen)

**Zweck**: Kerninfrastruktur, die VOR jeder User Story fertig sein MUSS

**⚠️ KRITISCH**: Keine User-Story-Arbeit darf beginnen, bevor diese Phase abgeschlossen ist

Beispiele für Grundlagen-Aufgaben (an dein Projekt anpassen):

- [ ] T004 Datenbankschema und Migrations-Framework einrichten
- [ ] T005 [P] Authentifizierungs-/Autorisierungs-Framework implementieren
- [ ] T006 [P] API-Routing und Middleware-Struktur einrichten
- [ ] T007 Basis-Modelle/-Entitäten erstellen, von denen alle Stories abhängen
- [ ] T008 Fehlerbehandlung und Logging-Infrastruktur konfigurieren
- [ ] T009 Umgebungs-Konfigurationsmanagement einrichten

**Checkpoint**: Grundlagen bereit – User-Story-Implementierung kann nun parallel beginnen

---

## Phase 3: User Story 1 - [Titel] (Priorität: P1) 🎯 MVP

**Ziel**: [Kurzbeschreibung, was diese Story liefert]

**Unabhängiger Test**: [Wie diese Story eigenständig verifiziert wird]

### Tests für User Story 1 (OPTIONAL - nur wenn Tests gefordert) ⚠️

> **HINWEIS: Diese Tests ZUERST schreiben, sicherstellen, dass sie VOR der Implementierung FEHLSCHLAGEN**

- [ ] T010 [P] [US1] Vertragstest für [Endpunkt] in src/test/java/contract/[name]Test.java
- [ ] T011 [P] [US1] Integrationstest für [Nutzerreise] in src/test/java/integration/[name]Test.java

### Implementierung für User Story 1

- [ ] T012 [P] [US1] [Entität1]-Modell in src/main/java/model/[entity1].java erstellen
- [ ] T013 [P] [US1] [Entität2]-Modell in src/main/java/model/[entity2].java erstellen
- [ ] T014 [US1] [Service] in src/main/java/service/[service].java implementieren (hängt ab von T012, T013)
- [ ] T015 [US1] [Endpunkt/Feature] in src/main/java/[ort]/[file].java implementieren
- [ ] T016 [US1] Validierung und Fehlerbehandlung ergänzen
- [ ] T017 [US1] Logging für die Operationen von User Story 1 ergänzen

**Checkpoint**: An diesem Punkt sollte User Story 1 voll funktionsfähig und unabhängig testbar sein

---

## Phase 4: User Story 2 - [Titel] (Priorität: P2)

**Ziel**: [Kurzbeschreibung, was diese Story liefert]

**Unabhängiger Test**: [Wie diese Story eigenständig verifiziert wird]

### Tests für User Story 2 (OPTIONAL - nur wenn Tests gefordert) ⚠️

- [ ] T018 [P] [US2] Vertragstest für [Endpunkt] in src/test/java/contract/[name]Test.java
- [ ] T019 [P] [US2] Integrationstest für [Nutzerreise] in src/test/java/integration/[name]Test.java

### Implementierung für User Story 2

- [ ] T020 [P] [US2] [Entität]-Modell in src/main/java/model/[entity].java erstellen
- [ ] T021 [US2] [Service] in src/main/java/service/[service].java implementieren
- [ ] T022 [US2] [Endpunkt/Feature] in src/main/java/[ort]/[file].java implementieren
- [ ] T023 [US2] Mit Komponenten von User Story 1 integrieren (falls nötig)

**Checkpoint**: An diesem Punkt sollten User Stories 1 UND 2 unabhängig funktionieren

---

[Weitere User-Story-Phasen nach demselben Muster ergänzen]

---

## Phase N: Feinschliff & Querschnittsthemen

**Zweck**: Verbesserungen, die mehrere User Stories betreffen

- [ ] TXXX [P] Dokumentations-Updates in docs/
- [ ] TXXX Code-Bereinigung und Refactoring
- [ ] TXXX Performance-Optimierung über alle Stories
- [ ] TXXX [P] Zusätzliche Unit-Tests (falls gefordert) in src/test/java/unit/
- [ ] TXXX Sicherheits-Härtung
- [ ] TXXX quickstart.md-Validierung durchführen

---

## Abhängigkeiten & Ausführungsreihenfolge

### Phasen-Abhängigkeiten

- **Einrichtung (Phase 1)**: Keine Abhängigkeiten – kann sofort starten
- **Grundlagen (Phase 2)**: Hängt von Einrichtung ab – BLOCKIERT alle User Stories
- **User Stories (Phase 3+)**: Hängen alle von der Grundlagen-Phase ab
  - User Stories können dann parallel laufen (wenn Kapazität da ist)
  - Oder sequenziell in Prioritäts-Reihenfolge (P1 → P2 → P3)
- **Feinschliff (letzte Phase)**: Hängt von allen gewünschten User Stories ab

### User-Story-Abhängigkeiten

- **User Story 1 (P1)**: Kann nach Grundlagen (Phase 2) starten – keine Abhängigkeiten zu anderen Stories
- **User Story 2 (P2)**: Kann nach Grundlagen (Phase 2) starten – darf mit US1 integrieren, aber unabhängig testbar bleiben
- **User Story 3 (P3)**: Kann nach Grundlagen (Phase 2) starten – darf mit US1/US2 integrieren, aber unabhängig testbar bleiben

### Innerhalb jeder User Story

- Tests (falls enthalten) MÜSSEN geschrieben werden und FEHLSCHLAGEN, bevor implementiert wird
- Modelle vor Services
- Services vor Endpunkten
- Kernimplementierung vor Integration
- Story abschließen, bevor zur nächsten Priorität gewechselt wird

### Parallel-Möglichkeiten

- Alle Einrichtungs-Aufgaben mit [P] können parallel laufen
- Alle Grundlagen-Aufgaben mit [P] können parallel laufen (innerhalb Phase 2)
- Nach Abschluss der Grundlagen-Phase können alle User Stories parallel starten (wenn Teamkapazität)
- Alle Tests einer User Story mit [P] können parallel laufen
- Modelle innerhalb einer Story mit [P] können parallel laufen
- Verschiedene User Stories können von verschiedenen Teammitgliedern parallel bearbeitet werden

---

## Implementierungsstrategie

### MVP zuerst (nur User Story 1)

1. Phase 1 abgeschlossen: Einrichtung
2. Phase 2 abgeschlossen: Grundlagen (KRITISCH – blockiert alle Stories)
3. Phase 3 abgeschlossen: User Story 1
4. **STOPP und VALIDIEREN**: User Story 1 unabhängig testen
5. Deployen/Demo, wenn bereit

### Inkrementelle Lieferung

1. Einrichtung + Grundlagen → Fundament bereit
2. User Story 1 → unabhängig testen → Deploy/Demo (MVP!)
3. User Story 2 → unabhängig testen → Deploy/Demo
4. User Story 3 → unabhängig testen → Deploy/Demo
5. Jede Story liefert Wert, ohne vorherige Stories zu brechen

### Parallele Team-Strategie

Mit mehreren Entwicklern:

1. Team erledigt Einrichtung + Grundlagen gemeinsam
2. Sobald Grundlagen fertig:
   - Entwickler A: User Story 1
   - Entwickler B: User Story 2
   - Entwickler C: User Story 3
3. Stories werden unabhängig abgeschlossen und integriert

---

## Hinweise

- [P]-Aufgaben = verschiedene Dateien, keine Abhängigkeiten
- [Story]-Label ordnet Aufgaben der jeweiligen User Story zu (Nachverfolgbarkeit)
- Jede User Story sollte unabhängig abschließbar und testbar sein
- Prüfen, dass Tests vor der Implementierung fehlschlagen
- Nach jeder Aufgabe oder logischen Gruppe committen
- An jedem Checkpoint anhalten, um die Story unabhängig zu validieren
- Vermeiden: vage Aufgaben, Konflikte in derselben Datei, story-übergreifende Abhängigkeiten, die die Unabhängigkeit brechen
