# custom-chat-server

TODO Beschreibung

### Projekt Struktur

Grundfunktionen
- ThreadPools und Worker für die asynchrone Verarbeitung von Anfragen
- Die Worker übernehmen die explizite Verarbeitung von Aufträgen indem sie z.B.: Daten in die 
- HTTPS/WS für Kommunikation zwischen Client und Server (openssl)
- Dynamimscher Wechsel zwischen HTTPS und WS je nach Bedarf. (Sobald der Chat aktiv ist wird auf WS geswitched)
- Separater Thread der Verbindungen entgegen nimmt und an ThreadPool verteilt.
- Anmeldung mit Benutzername/Passwort, Authentifizierung mit Cookies (JWT-Tokens?)
- Key-Pair wird (mit Passwort verschlüsselt) auf Server Seite gespeichert
- Passwort wird gehashed auf Server gespeichert
- Benutzer kriegen eine UUID
- Schnittstellen zwischen Server und Client werden durch eine REST-API definiert
- Orientierung der API an Zulip


 
|M| -- |H| --> [TP1[W1, W2, W3], TP2[W4, W5, W6]] 
