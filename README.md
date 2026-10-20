# Eltern-Infoportal Medienkompetenz

Eine schlanke Linkseite für Eltern, die in vier Schritten durch das Thema führt. Kein Konto bei Canva oder Bio.link nötig.

## Dateien

- `index.html`: die Seite. Muss in der Regel nicht verändert werden.
- `links.json`: alle Texte, Schritte und Links. Hier wird gepflegt.
- `logo.svg`: das Logo.
- `README.md`: diese Anleitung.

## Aufbau der Seite

1. **Startfragen:** drei Schaltflächen, die direkt zu einem Schritt springen.
2. **Journey:** vier Schritte: Eltern informieren, Kind informieren, Einstellungen treffen, Begleiten und dranbleiben.
3. **Altersfilter:** Eltern wählen „Vorschule“, „1./2. Klasse“ oder „3./4. Klasse“. Links für andere Altersgruppen werden ausgeblendet. Links mit „Alle“ bleiben immer sichtbar.
4. **Fußbereich:** Stand, Kontakt und Impressum.

## Inhalte ändern

1. Auf GitHub die Datei `links.json` öffnen.
2. Auf das Stift-Symbol (Edit) klicken.
3. Text ändern oder einen Link ergänzen. Ein Link sieht so aus:

```json
{
  "titel": "Titel des Links",
  "url": "https://www.beispiel.de/",
  "beschreibung": "Ein Satz, was Eltern dort bekommen.",
  "format": "text",
  "alter": ["alle"],
  "region": "bundesweit"
}
```

**Erlaubte Werte:**

- `format`: `text`, `video`, `audio`, `pdf`, `buch`, `tool`, `beratung`
- `alter`: `"alle"`, `"vorschule"`, `"1-2"`, `"3-4"`. Mehrere Werte sind möglich, z. B. `["1-2", "3-4"]`.
- `region`: `"bundesweit"` oder ein Bundesland, z. B. `"Bayern"`. Nicht-bundesweite Angebote zeigen den Hinweis „Nur Bayern“ an.

**Achtung:** Zwischen zwei Links steht ein Komma, beim letzten Link der Liste nicht. Anführungszeichen `"` bleiben erhalten.

4. Unten auf **Commit changes** klicken. Nach ein bis zwei Minuten ist die Änderung online.

**Pflege:** Bitte beim Ändern auch `zuletzt_aktualisiert` im Abschnitt `profil` auf den aktuellen Monat setzen.

## Kontakt und Impressum

Im Abschnitt `profil` gibt es zwei Felder:

- `kontakt`: eine E-Mail-Adresse, damit Eltern tote Links oder Fehler melden können.
- `impressum_url`: Link zu einer Impressum-Seite, z. B. der Schulwebsite.

Leere Felder werden nicht angezeigt. Ob für das Angebot ein Impressum nötig ist, bitte mit der Schule oder dem Träger klären.

## Einmalige Veröffentlichung auf GitHub Pages

1. Auf github.com ein Repository `eltern-infoportal` anlegen (Public).
2. Alle Dateien hochladen und **Commit changes** klicken.
3. Unter **Settings → Pages** bei **Source** die Option **Deploy from a branch** wählen, Branch `main`, Ordner `/ (root)`, dann **Save**.
4. Die Adresse steht danach oben auf der Pages-Seite, z. B. `https://<benutzername>.github.io/eltern-infoportal/`.

## Weitere Administratoren hinzufügen

1. Im Repository auf **Settings → Collaborators** gehen.
2. **Add people** klicken und das GitHub-Konto der Person eintragen.
3. Die Person kann danach `links.json` direkt bearbeiten.

## Vor jeder Veröffentlichung prüfen

- Jeden Link einmal selbst anklicken.
- Die Seite auf dem Smartphone öffnen.
- Die Altersangaben und Regionen stimmen lassen.
- Lokal per Doppelklick zeigt die Seite keine Links an. Die Vorschau funktioniert erst über die GitHub-Pages-Adresse.
