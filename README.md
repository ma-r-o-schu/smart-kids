# Eltern-Infoportal Medienkompetenz

Eine einfache, kostenlose Linkseite (ähnlich Bio.link), die ohne Canva- oder Bio.link-Konto auskommt.

## Dateien

- `index.html` – die Seite. Muss in der Regel nicht verändert werden.
- `links.json` – alle Texte, Kategorien und Links. Hier wird gepflegt.
- `README.md` – diese Anleitung.

## Inhalte ändern (ohne Programmierkenntnisse)

1. Auf GitHub die Datei `links.json` öffnen.
2. Auf das Stift-Symbol (Edit) klicken.
3. Text ändern oder einen Link ergänzen. Ein Link-Block sieht so aus:

```json
{
  "titel": "🔗 Titel des Links",
  "url": "https://www.beispiel.de/",
  "beschreibung": "Kurze Erklärung für Eltern."
}
```

Achtung: Zwischen den Blöcken steht ein Komma, der letzte Block einer Liste hat keines. Die Anführungszeichen `"` bleiben stehen.

4. Unten auf **Commit changes** klicken. Nach ein bis zwei Minuten ist die Änderung online.

## Einmalige Veröffentlichung auf GitHub Pages

1. Auf github.com ein kostenloses Konto anlegen oder einloggen.
2. Oben rechts auf **+** → **New repository** klicken. Name z. B. `eltern-infoportal`, Sichtbarkeit **Public**.
3. Auf **uploading an existing file** klicken und die Dateien `index.html`, `links.json` und `README.md` hochladen. Dann **Commit changes**.
4. Im Repository auf **Settings** → **Pages** gehen. Unter **Build and deployment** als Quelle **Deploy from a branch**, Branch **main**, Ordner **/ (root)** wählen und speichern.
5. Nach kurzer Zeit erscheint die Adresse `https://<benutzername>.github.io/eltern-infoportal/`. Diese Adresse kann an Eltern verteilt werden.

## Andere Personen als Administratoren hinzufügen

1. Im Repository auf **Settings** → **Collaborators** (bzw. **Collaborators and teams**) gehen.
2. **Add people** klicken und das GitHub-Konto der Person eingeben.
3. Die Person erhält eine Einladung und kann danach `links.json` direkt bearbeiten, wie oben beschrieben.

## Hinweise

- Vor dem Veröffentlichen die Links einmal selbst anklicken, da Webseiten sich ändern.
- Die Bio und der Profil-Titel stehen am Anfang der Datei `links.json` unter `profil`.
- Die Seite funktioniert auf dem Smartphone und im Dunkelmodus.
- Lokal im Browser per Doppelklick geöffnet, zeigt die Seite wegen einer Browser-Sperre keine Links an. Sie funktioniert erst über die GitHub-Pages-Adresse oder einen kleinen lokalen Server.
