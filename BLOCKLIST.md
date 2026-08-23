# blocklist.json

SHK IPTV lädt diese Datei automatisch und verweigert die Verbindung zu jedem
hier gelisteten Server (siehe Nutzungsbedingungen, Punkt 3). Eine Domain in
der Liste sperrt automatisch auch alle ihre Subdomains.

Format: ein einfaches JSON-Array aus Hostnamen, kein Wrapper-Objekt.

```json
["beispiel-anbieter.tld", "noch-einer.tld"]
```

## Einen Eintrag hinzufügen

1. Domain in `blocklist.json` ergänzen, committen, nach `main` pushen.
2. Fertig - kein neuer App-Release nötig. Installierte Apps laden die Liste
   selbstständig neu (Cache-Dauer: 24h).

## Wann ein Eintrag hier reingehört

Nur mit tatsächlicher Grundlage - z. B. eine Sperrverfügung, eine konkrete
Meldung eines Rechteinhabers, oder anderweitig belastbare Kenntnis, dass ein
Anbieter Inhalte ohne die erforderlichen Rechte anbietet. Nicht auf bloßen
Verdacht hin - ein fälschlich gesperrter, tatsächlich legitimer Anbieter
richtet mehr Schaden an als ein verspätet gesperrter.
