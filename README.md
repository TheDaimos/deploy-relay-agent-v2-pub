# Deploy Relay Agent V2 — Öffentliche Entwicklung

**Status: Entwicklungsvorbereitung. Noch keine V2-Freigabe, kein veröffentlichter V2-Installationsstand.**

Dieses Repository ist die **öffentliche Entwicklungsquelle** für die nächste Ausführungsarchitektur von Deploy Relay Agent (DRA), einer Home-Assistant-Integration zur kontrollierten Bereitstellung ausgewählter Git-Stände.

## Ausgangsbasis

Der Quellcode unter `custom_components/deploy_relay/` wird aus dem **bereits öffentlichen** [DRA-V1-HACS-Repository](https://github.com/TheDaimos/deploy-relay-agent-pub) übernommen und zunächst **bytegleich** als nachvollziehbare Ausgangsbasis eingefroren.

- Quelle: `TheDaimos/deploy-relay-agent-pub`, Commit `0c9d7f49f080dfe77b6c3910f89d6a61ae4b8cfa`.
- Ausgangsversion: **1.0.0**, nicht als V2-Version umdeuten.
- Neues Repository, **neue Git-Historie**: keine Übernahme der privaten DEV-Geschichte, privaten Diagnosen, lokalen Sicherungen oder Zugangsdaten.
- Die öffentliche [V1-HACS-Auslieferung](https://github.com/TheDaimos/deploy-relay-agent-pub) bleibt davon unabhängig.

**Bitte dieses Repository noch nicht über HACS oder DRA zur Aktualisierung einer produktiv genutzten Installation verwenden.** Die V2-Entwicklung beginnt erst nach der getrennten V1-Finalisierung und den vorgeschriebenen Abnahmen.

## Geplanter V2-Umbau

- Aufträge dauerhaft serverseitig führen, statt vom geöffneten Browser abhängig zu sein.
- Auftrag, Fortschritt, Sperr-/Wartezustand und Ergebnis nachvollziehbar speichern.
- Verbindungsausfall und erneute Verbindung ohne Verlust des Auftragsstatus ermöglichen.
- Sammelprüfungen und Sammelinstallation auf dem Home-Assistant-Server steuern.
- Große Dateilisten bedarfsgerecht übertragen; Mobilgeräte entlasten.
- Vorhandene Schreibsperren, Backup-vor-Mutation, Prüfung, Rückfall und Wiederherstellungszustände **nicht abschwächen**.
- Diagnose und Protokolle mit gemeinsamen, bereinigten Ereignisdaten ausstatten.
- Home-Assistant-Integrationsansicht, offizielle DRA-Logos und Zugang ohne sichtbaren Seitenleisteneintrag verbessern.

Der grobe öffentliche Entwicklungsplan steht in [docs/V2_ROADMAP.md](docs/V2_ROADMAP.md); verbindliche Prüf- und Freigabeschritte werden vor Implementierungsbeginn dokumentiert.

## Sicherheit und Veröffentlichung

[PUBLIC_DEVELOPMENT_POLICY.md](docs/PUBLIC_DEVELOPMENT_POLICY.md) regelt die Veröffentlichung. Keine Tokens, Geheimnisse, Hostnamen privater Systeme, IP-Adressen, personenbezogene Diagnosen, Home-Assistant-Konfiguration, Sicherungen oder Inhalte privater Erweiterungen in diesem Repository oder seinen Actions-Protokollen.

Der Projektcode unterliegt **GPL-3.0-only**; offizielle Projektlogos und Namensrechte sind gemäß [BRANDING.md](BRANDING.md) gesondert geschützt. Siehe auch [COPYRIGHT.md](COPYRIGHT.md), [AUTHORS.md](AUTHORS.md) und [THIRD_PARTY.md](THIRD_PARTY.md).

## Automatische Prüfungen

Die öffentlichen Standard-GitHub-Runner prüfen vorerst Quellintegrität, Syntax, Lizenz-/Paketgrenzen und wichtige Sicherheitsverträge. **Kein automatischer Artefaktupload**, um den bestehenden GitHub-Artefaktspeicher nicht zusätzlich zu belasten.

Automatische Prüfungen ersetzen keine reale Home-Assistant-Abnahme. CI-Ergebnisse und Versionskennungen dürfen nicht als V2-Freigabe verstanden werden.

**C.K. – Eine Idee weiter gedacht.**
