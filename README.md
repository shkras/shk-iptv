# SHK IPTV

SHK IPTV ist eine App zum Streamen deiner IPTV-Kanäle – für Windows, macOS und Linux.

## Installation

Aktuelle Version auf der [Releases-Seite](../../releases):

### Windows

- **Installer** (`SHK-IPTV-Setup-X.Y.Z.exe`) – empfohlen, mit Startmenü-Eintrag, normale Deinstallation über Windows.
- **Portable** (`.zip`) – kein Setup, einfach entpacken und starten.

Windows 10/11, 64-bit.

Beim ersten Start zeigt Windows evtl. eine Warnung ("Unbekannter Herausgeber"). Das ist normal, kein Sicherheitsproblem – auf "Weitere Informationen" → "Trotzdem ausführen" klicken.

### macOS

- **`.dmg`** – empfohlen, öffnen und in den Programme-Ordner ziehen.
- **`.zip`** – alternativ, einfach entpacken und starten.

Apple Silicon (arm64), macOS 11+.

Da wir kein Apple-Entwicklerzertifikat haben, ist die App nicht signiert. macOS meldet beim ersten Start deshalb, sie sei "beschädigt" und gehöre in den Papierkorb – das ist keine echte Beschädigung, sondern Gatekeeper. Im Terminal die Quarantäne-Markierung entfernen, dann startet sie normal:

```
xattr -cr "/Applications/SHK IPTV.app"
```

(Pfad anpassen, falls die App nicht im Programme-Ordner liegt.) Der Weg über Systemeinstellungen → Datenschutz & Sicherheit → "Trotzdem öffnen" funktioniert bei unsignierten Apps wie dieser oft nicht – dann bringt nur der Terminal-Befehl.

### Linux

- **`.AppImage`** – herunterladen, ausführbar machen (`chmod +x SHK-IPTV-*.AppImage`) und starten.

x86_64.

## Erste Schritte

Zugangsdaten (Server, Benutzername, Passwort) einmal eingeben, die App merkt sich alles für den nächsten Start. Vor dem ersten Start müssen die [Nutzungsbedingungen](NUTZUNGSBEDINGUNGEN.md) akzeptiert werden.

## Funktionen

- Senderliste mit Suche und Favoriten
- Programmführer
- Verbindungsqualitäts-Anzeige während der Wiedergabe
- Automatische Updates
- Deine Zugangsdaten werden ausschließlich lokal und verschlüsselt gespeichert

## Häufige Fragen

**Ein Sender startet nicht oder bricht ab.**
Meist liegt es am Signal, nicht an der App. Meld dich bei uns, wenn es öfter vorkommt.

**Die App öffnet sich kein zweites Mal.**
Das ist Absicht – ein erneuter Start holt einfach das laufende Fenster nach vorne.

**Nach einem Wechsel zwischen Installer- und portabler Version sind meine Daten weg.**
Beide Varianten speichern getrennt. Einmal neu anmelden genügt.

## Kontakt

Fragen oder Probleme? Über die [Issues-Seite](../../issues) melden.

---

© 2026 SHK. Alle Rechte vorbehalten. Nutzt [FFmpeg](https://ffmpeg.org) für die Audiowiedergabe – Details siehe [LICENSE](LICENSE) und [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
