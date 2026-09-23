# Einfaches Browser-Stimmgerät

Ein kleines chromatisches Stimmgerät, das direkt im Browser läuft. Kein Server und keine Installation nötig.

## GitHub Pages

1. Neues GitHub-Repository anlegen, z. B. `stimmgeraet`.
2. `index.html` in das Repository hochladen.
3. In GitHub: **Settings → Pages**.
4. Unter **Build and deployment** als Source **Deploy from a branch** wählen.
5. Branch `main` und Ordner `/ (root)` auswählen und speichern.
6. Nach dem Deployment die angezeigte `https://...github.io/...`-Adresse öffnen und teilen.

## iPhone

- Am besten mit Safari öffnen.
- Auf **Mikrofon starten** tippen.
- Mikrofonzugriff erlauben.
- GitHub Pages nutzt HTTPS; das ist für den Mikrofonzugriff erforderlich.

## Funktionen

- chromatische Notenerkennung
- Frequenzanzeige
- Cent-Abweichung mit Nadel
- Referenzton A4 einstellbar, Standard 440 Hz
- keine Datenübertragung: Audio wird nur lokal im Browser ausgewertet
