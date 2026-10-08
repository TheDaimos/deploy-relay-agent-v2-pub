# Öffentlicher Ursprung des vorbereiteten V2-Veröffentlichungskanals

Stand: 08.10.2026. **Noch keine V2-Version veröffentlicht.**

| Ebene | Quellstand |
| --- | --- |
| Bereits öffentlich veröffentlichte V1.0.0-Basis | `TheDaimos/deploy-relay-agent-pub@0c9d7f49f080dfe77b6c3910f89d6a61ae4b8cfa` |
| Nachweisbarer Import in dieses Repository | `c67bed1d9a4eb669796b6831c65534d956826794` |
| Verifizierte Basispaketdateien | 43 byte-/Git-Blob-identische V1-Dateien, einschließlich vollständiger Integration und öffentlicher Lizenz-/Sicherheitsunterlagen |
| Offizielle Bilddateien | `brand/icon.png` und `brand/icon@2x.png` unverändert |
| Private Git-Historie, private Diagnosen und Zugangsdaten | **Nicht übernommen** |
| Laufende V2-Entwicklung | `TheDaimos/deploy-relay-agent-v2-dev` – separates öffentliches Repository |
| Veröffentlichungsstatus | `NOT RELEASED`, aktuelle Laufzeitbasis weiter `1.0.0` |

Der initiale öffentliche Stagingstand wurde für `v2-dev` in einer weiteren, eigenständigen Git-Historie übernommen. Dieses Repository wird ab jetzt für kontrollierte, **explizit abgenommene** V2-Veröffentlichungen reserviert und nicht als täglicher Entwicklungszweig betrieben.

Die privaten V1-Quellen, alten Git-Commits, Tests mit realen Daten, Home-Assistant-Sicherungen und Diagnoseexporte wurden nicht importiert.

## Prüfpflicht für spätere Veröffentlichungen

Jede Übernahme aus `v2-dev` verlangt einen eindeutigen DEV-Quellcommit, ein belegtes unverändertes Stagingpaket, HACS-/Hassfest-Prüfungen, gesicherte V1→V2-Migration, reale HA-Abnahme und bewusste Freigabe. Keine Aktualisierung über einen beweglichen DEV-Zweig direkt in den Veröffentlichungskanal.
