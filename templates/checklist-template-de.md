# [CHECKLISTEN-TYP] Checkliste: [FEATURE-NAME]

**Zweck**: [Kurzbeschreibung, was diese Checkliste abdeckt]
**Erstellt**: [DATUM]
**Feature**: [Link zu spec.md oder relevanter Dokumentation]

**Hinweis**: Diese benutzerdefinierte Checkliste wird vom Befehl `__SPECKIT_COMMAND_CHECKLIST__` basierend auf Feature-Kontext und Anforderungen generiert.
**Review-Verantwortung**: Diese Checkliste ist ein reviewer-eigenes Artefakt zur Qualitätsprüfung der Anforderungen. Ein Element `[x]` nur markieren, wenn der Reviewer feststellt, dass das Anforderungs-Qualitätskriterium erfüllt ist.
**Marker-Semantik**: `[x]` bedeutet, dass das Kriterium geprüft und für die Anforderungsqualität erfüllt wurde. Es bedeutet NICHT, dass die Implementierungsarbeit abgeschlossen ist.

<!--
  ============================================================================
  WICHTIG: Die Checklisten-Elemente unten sind BEISPIEL-Elemente nur zur Veranschaulichung.

  Der Befehl __SPECKIT_COMMAND_CHECKLIST__ MUSS diese durch echte Elemente ersetzen, basierend auf:
  - Der konkreten Checklisten-Anfrage des Nutzers
  - Feature-Anforderungen aus spec.md
  - Technischem Kontext aus plan.md
  - Implementierungsdetails aus tasks.md

  Diese Beispiel-Elemente NICHT in der generierten Checklisten-Datei behalten.
  ============================================================================
-->

## [Kategorie 1]

- [ ] CHK001 Erstes Checklisten-Element mit klarer Aktion
- [ ] CHK002 Zweites Checklisten-Element
- [ ] CHK003 Drittes Checklisten-Element

## [Kategorie 2]

- [ ] CHK004 Weiteres Kategorie-Element
- [ ] CHK005 Element mit konkreten Kriterien
- [ ] CHK006 Letztes Element dieser Kategorie

## Hinweise

- Elemente erst `[x]` markieren, wenn die Prüfung bestätigt, dass das Anforderungs-Qualitätskriterium erfüllt ist
- Elemente unmarkiert lassen, solange sie Klärung, Korrektur oder Reviewer-Bewertung erfordern
- `__SPECKIT_COMMAND_IMPLEMENT__` liest den Checkbox-Status als Gate und darf keine Marker ändern
- `checklists/requirements.md` hat einen separaten eingebauten Lebenszyklus, gepflegt von `__SPECKIT_COMMAND_SPECIFY__` und `__SPECKIT_COMMAND_CLARIFY__`
- Kommentare oder Befunde inline ergänzen
- Auf relevante Ressourcen oder Dokumentation verlinken
- Elemente sind fortlaufend nummeriert für einfache Referenz
