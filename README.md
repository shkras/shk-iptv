# SHK IPTV

Eine Windows-Anwendung zum Streamen von IPTV-Inhalten über einen Xtream-Codes-Zugang.

Dieses Repository enthält ausschließlich die fertigen Downloads (Installer/Programm) und Nutzer-Dokumentation - kein Quellcode.

## Download & Installation

Die aktuelle Version findest du auf der [Releases-Seite](../../releases):

- **`SHK IPTV Setup X.Y.Z.exe`** - Installer (empfohlen). Führt durch eine normale Windows-Installation, legt eine Verknüpfung im Startmenü an und lässt sich über *Einstellungen → Apps* wie jedes andere Programm wieder deinstallieren.
- **`SHK-IPTV-vX.Y.Z-portable-win-x64.zip`** - Portable Variante ohne Installation. Einfach entpacken und `SHK IPTV.exe` starten. Praktisch, wenn du keine Installation vornehmen möchtest oder die App von einem USB-Stick aus nutzen willst.

**Systemvoraussetzungen:** Windows 10 oder 11 (64-bit).

### Warnung "Unbekannter Herausgeber" / SmartScreen

Beim ersten Start des Installers (oder der `.exe`) zeigt Windows möglicherweise eine blaue SmartScreen-Warnung ("Windows hat den Computer geschützt" / "Unbekannter Herausgeber"). Das liegt daran, dass die App nicht mit einem kostenpflichtigen Code-Signing-Zertifikat signiert ist - **nicht** an einem Sicherheitsproblem. Zum Fortfahren auf **"Weitere Informationen"** und dann **"Trotzdem ausführen"** klicken.

## Erste Schritte

Für die Nutzung wird ein bestehender **Xtream-Codes-IPTV-Zugang** benötigt (Server-Adresse, Benutzername, Passwort) - erhältlich bei einem IPTV-Anbieter. Diese App ist nur ein Wiedergabe-Programm und liefert selbst keine Inhalte.

Beim ersten Start werden Server, Benutzername und Passwort abgefragt und danach lokal für den nächsten Start gespeichert.

## Funktionen

- Senderliste mit Kategorien, Live-Suche und Favoriten
- Programmführer (EPG) mit aktueller und kommender Sendung
- Automatische Tonspur-Kompatibilität - manche Anbieter liefern Sender in einem Audioformat, das Windows-Browser nicht direkt abspielen können; SHK IPTV gleicht das automatisch aus, ohne die Bildqualität zu verändern
- Verbindungsqualitäts-Anzeige während der Wiedergabe
- Automatische Updates (siehe unten)
- Dark-Theme-Oberfläche

## Datenschutz & Sicherheit

- Zugangsdaten werden **ausschließlich lokal auf deinem Gerät** gespeichert, verschlüsselt über den in Windows eingebauten Schutzmechanismus für den angemeldeten Benutzer. Eine kopierte Datei ist auf einem anderen Gerät oder unter einem anderen Benutzerkonto unbrauchbar.
- Es gibt keine Cloud-Anbindung, kein Nutzerkonto bei SHK IPTV und kein Tracking. Die App verbindet sich ausschließlich direkt mit dem von dir eingetragenen IPTV-Server.
- Eine Deinstallation entfernt auch alle lokal gespeicherten Daten (Zugangsdaten, Favoriten, Verlauf, Einstellungen).

## Automatische Updates

SHK IPTV prüft beim Start automatisch auf neue Versionen. Eine gefundene Aktualisierung wird im Hintergrund heruntergeladen und beim nächsten regulären Neustart der App installiert - ohne Unterbrechung der laufenden Nutzung. Eine manuelle Prüfung ist über *Einstellungen → "Nach Updates suchen"* möglich.

## Problembehandlung

**"Unbekannter Herausgeber"-Warnung beim Start** - siehe oben, das ist erwartet und unbedenklich.

**Ein Sender lädt nicht oder bricht ab** - meist liegt es am IPTV-Anbieter selbst, nicht an der App. Zur Kontrolle: den gleichen Sender testweise in einem anderen Player (z. B. VLC) öffnen - tritt das Problem dort ebenfalls auf, liegt es am Anbieter.

**Die App öffnet sich nicht ein zweites Mal** - das ist beabsichtigt: SHK IPTV läuft immer nur einmal gleichzeitig. Ein erneuter Start holt das bereits laufende Fenster nach vorne, statt eine zweite Instanz zu öffnen.

**Zugangsdaten sind nach einem Umstieg von der portablen auf die installierte Version (oder umgekehrt) weg** - beide Varianten speichern ihre Daten bewusst getrennt voneinander. Einfach einmal neu anmelden, die Daten werden danach wieder gespeichert.

## Danksagung

SHK IPTV nutzt [FFmpeg](https://ffmpeg.org) (lizenziert unter LGPL/GPL) für die automatische Tonspur-Kompatibilität.

## Fragen & Feedback

Über die [Issues-Seite](../../issues) dieses Repositories.
