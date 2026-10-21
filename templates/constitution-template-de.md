# [PROJEKTNAME] Verfassung (Constitution)
<!-- Beispiel: Spec-Verfassung, TaskFlow-Verfassung usw. -->

## Kernprinzipien

### [PRINZIP_1_NAME]
<!-- Beispiel: I. Library-First -->
[PRINZIP_1_BESCHREIBUNG]
<!-- Beispiel: Jedes Feature startet als eigenständige Bibliothek; Bibliotheken müssen in sich geschlossen, unabhängig testbar und dokumentiert sein; klarer Zweck erforderlich – keine rein organisatorischen Bibliotheken -->

### [PRINZIP_2_NAME]
<!-- Beispiel: II. CLI-Schnittstelle -->
[PRINZIP_2_BESCHREIBUNG]
<!-- Beispiel: Jede Bibliothek stellt Funktionalität über CLI bereit; Text-Ein/Ausgabe-Protokoll: stdin/args → stdout, Fehler → stderr; JSON + menschenlesbare Formate unterstützen -->

### [PRINZIP_3_NAME]
<!-- Beispiel: III. Test-First (NICHT VERHANDELBAR) -->
[PRINZIP_3_BESCHREIBUNG]
<!-- Beispiel: TDD verpflichtend: Tests geschrieben → Nutzer genehmigt → Tests schlagen fehl → dann implementieren; Red-Green-Refactor-Zyklus strikt durchsetzen -->

### [PRINZIP_4_NAME]
<!-- Beispiel: IV. Integrationstests -->
[PRINZIP_4_BESCHREIBUNG]
<!-- Beispiel: Fokusbereiche, die Integrationstests erfordern: neue Bibliotheks-Vertragstests, Vertragsänderungen, Service-übergreifende Kommunikation, gemeinsame Schemata -->

### [PRINZIP_5_NAME]
<!-- Beispiel: V. Observability, VI. Versionierung & Breaking Changes, VII. Einfachheit -->
[PRINZIP_5_BESCHREIBUNG]
<!-- Beispiel: Text-I/O gewährleistet Debuggbarkeit; strukturiertes Logging erforderlich; Oder: MAJOR.MINOR.BUILD-Format; Oder: einfach anfangen, YAGNI-Prinzip -->

## [ABSCHNITT_2_NAME]
<!-- Beispiel: Zusätzliche Einschränkungen, Sicherheitsanforderungen, Leistungsstandards usw. -->

[ABSCHNITT_2_INHALT]
<!-- Beispiel: Anforderungen an den Technologie-Stack, Compliance-Standards, Deployment-Richtlinien usw. -->

## [ABSCHNITT_3_NAME]
<!-- Beispiel: Entwicklungsworkflow, Review-Prozess, Qualitäts-Gates usw. -->

[ABSCHNITT_3_INHALT]
<!-- Beispiel: Code-Review-Anforderungen, Test-Gates, Freigabeprozess für Deployments usw. -->

## Governance
<!-- Beispiel: Die Verfassung steht über allen anderen Praktiken; Änderungen erfordern Dokumentation, Freigabe und Migrationsplan -->

[GOVERNANCE_REGELN]
<!-- Beispiel: Alle PRs/Reviews müssen die Konformität prüfen; Komplexität muss begründet werden; [LEITFADEN_DATEI] für Laufzeit-Entwicklungsleitlinien verwenden -->

**Version**: [VERFASSUNGS_VERSION] | **Ratifiziert**: [RATIFIZIERUNGSDATUM] | **Zuletzt geändert**: [DATUM_LAST_AMENDED]
<!-- Beispiel: Version: 2.1.1 | Ratifiziert: 2025-06-13 | Zuletzt geändert: 2025-07-16 -->
