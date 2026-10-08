# Verbindliche Veröffentlichungsregeln – DRA V2 Public

## Aufgabe

`TheDaimos/deploy-relay-agent-v2-pub` ist **ausschließlich** der Veröffentlichungskanal für freigegebene DRA-V2-Versionen. Die gesamte normale Entwicklung samt CI findet im ebenfalls öffentlichen `TheDaimos/deploy-relay-agent-v2-dev` statt.

**Aktueller Zustand: noch kein V2-FINAL.** Die in diesem Repository liegenden `1.0.0`-Quelldateien sind nur die bereits veröffentlichte V1-Ausgangsbasis.

## Freigabegates

1. Verbindliche DEV-Version, konkrete Commit-SHA und vollständige Änderungs-/Bestandsübersicht festhalten.
2. Alle automatisierten Prüfungen im V2-DEV-Repository grün, einschließlich Sicherheits-, Ressourcen-, Transaktions-, Migrations-, HACS- und Hassfest-Prüfungen soweit relevant.
3. Reale Home-Assistant-Abnahme von Installation, Update, Projekterhaltung, Zugriffssicherheit, Sicherung, Verifikation, Rollback und Neustartmaßnahmen dokumentieren.
4. Öffentliche Quellinhalte und alle Verzeichnisänderungen erneut auf Zugangsdaten, personenbezogene Informationen, private Diagnoseexporte und private Erweiterungen prüfen.
5. Nur das freigegebene Paket aus dem DEV-Commit übernehmen; Git-Prüfwerte und publizierten Versionsstand vergleichen.
6. Versions-/Kanalhinweise, HACS-Metadaten, Installations- und Freigabedokumentation aktualisieren.
7. **Ausdrückliche Freigabe durch den Projektinhaber** einholen. Erst anschließend gezieltes Tag-/Release-/HACS-Verfahren.
8. Nach Veröffentlichung realen Aktualisierungs-/Rückfalltest sowie den unveränderten V1-HACS-Kanal prüfen.

## Automatisierung und Sicherheit

Kein automatisches Spiegeln von DEV nach PUB, keine ungenehmigte Releaseaktion, kein PR-getriebener Produkthochlauf. Standard-GitHub-Runner nur mit minimalen Berechtigungen. Builds/Artefakte lediglich nach Bedarf; kein dauernder Upload von Testpaketen.

## Rechtliches

Der Softwarecode ist GPL-3.0-only. Die offiziellen Marken- und Bildrechte verbleiben gemäß BRANDING.md beim Projektinhaber. Private Git-Historie, Geheimnisse, personenbezogene Diagnosen, Home-Assistant-Konfiguration oder Sicherungen gehören grundsätzlich nicht in öffentliche Auslieferungen.
