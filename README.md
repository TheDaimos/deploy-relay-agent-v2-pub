# Deploy Relay Agent V2 — öffentlicher Veröffentlichungskanal

**Status: V2 noch nicht veröffentlicht. Dieses Repository ist derzeit nur vorbereitet, nicht als V2-HACS-Quelle freigegeben.**

Dieses Repository ist der künftig **stabile öffentliche Auslieferungskanal** für Deploy Relay Agent V2 (Home Assistant).

## Saubere Trennung

- **[deploy-relay-agent-v2-dev](https://github.com/TheDaimos/deploy-relay-agent-v2-dev):** Laufende Entwicklung, Fehlerkorrekturen, automatische Prüfungen, Teststände, verbindliche Architektur- und Abnahmearbeit.
- **[deploy-relay-agent-v2-pub](https://github.com/TheDaimos/deploy-relay-agent-v2-pub):** Nur nach ausdrücklicher Freigabe übernommene V2-Stände, späterer HACS-Veröffentlichungskanal.
- **[deploy-relay-agent-pub](https://github.com/TheDaimos/deploy-relay-agent-pub):** Bestehende V1-HACS-Auslieferung; bleibt während der V2-Entwicklung unverändert.

## Aktueller Inhalt

Der Integrationsordner ist eine **bereits öffentlich veröffentlichte V1.0.0-Quellbasis** mit den offiziellen DRA-Markengrafiken. Die vorbereitenden V2-Dateien begründen **keine V2-Version**. Eine HACS-V2-Freigabe ist noch nicht erfolgt. **Bitte dieses Repository gegenwärtig nicht als V2-Installationsquelle verwenden.**

Die bisherige private Git-Historie, private Entwicklungsdiagnosen und lokale Home-Assistant-Daten sind nicht in dieses Repository eingeflossen. Siehe [öffentliche Ausgangsbasis](docs/SOURCE_PROVENANCE.md).

## Zukünftige Veröffentlichungen

Eine Version gelangt ausschließlich nach bestandenen Tests, vollständig dokumentierter Home-Assistant-Realabnahme, Sicherheits-/Ressourcenprüfung und expliziter Release-Freigabe aus dem öffentlichen `v2-dev` nach `v2-pub`. Jede Übernahme wird über einen konkreten Commit-SHA und die geprüften Datei-Prüfwerte dokumentiert.

**Keine automatische Synchronisierung, kein automatischer Versionssprung und kein stiller HACS-Release.** Die Einzelheiten stehen in [PUBLIC_RELEASE_POLICY.md](docs/PUBLIC_RELEASE_POLICY.md).

Die Software steht unter GPL-3.0-only; für offizielle Logos und Marken gelten [BRANDING.md](BRANDING.md) und [COPYRIGHT.md](COPYRIGHT.md).

**C.K. – Eine Idee weiter gedacht.**
