# Git

![](git.svg)

## Installation

1. 📥 https://git-scm.com/downloads
   - ⚠️ Während der Installation als Editor **nano** auswählen (meist ganz oben; hochscrollen) ⚠️
2. Im Windows-Startmenü `Git Bash` eingeben und starten
3. Git-Verzeichnis anlegen und betreten
   - `mkdir git`
   - `cd git`

## Tutorial

- 📥 https://code.visualstudio.com/Download
- 📺 https://www.youtube.com/watch?v=9IINVQ5wx0c
- Einführung bis 6:00 passiv schauen
- Ab 6:00 aktiv mitmachen
- Falls `code` ab 8:50 nicht funktioniert, habt ihr VS Code nicht installiert
  - Laufende Git Bash schließen
  - 📥 https://code.visualstudio.com/Download
  - Neue Git Bash öffnen
- Ab 42:37 wird per HTTPS mit GitHub kommuniziert; am 13. August 2021 hat GitHub den Upload per HTTPS jedoch abgeschaltet! Mögliche Lösungen:
  - [Personal Access Token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
  - [SSH statt HTTPS](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
  - GitLab statt GitHub
  - BitBucket statt GitHub

## Workflow für Anfänger (ohne lokale Branches, Merge statt Rebase)

1. Im Windows-Startmenü `Git Bash` eingeben und starten
2. Projekt-Verzeichnis betreten
   - `cd git/beispiel`
3. Neue Commits der Kollegen herunterladen
   - `git pull`
4. Ein konkretes Feature umsetzen oder einen konkreten Bug fixen
5. Lokale Änderungen stagen und committen
   - `git add .`
   - `git commit -m "Sinnvolle Beschreibung des Features bzw. Bugfix"`
6. Neuen Commit hochladen
   - `git push`
   - **Funktioniert?** Feierabend bzw. Zurück zu Schritt 4
7. Neue, potenziell konfligierende Commits der Kollegen herunterladen
   - `git pull`
   - **Funktioniert?** Zurück zu Schritt 6
8. Mit Merge-Konflikten umgehen
   - **Konflikte in der IDE manuell beheben** (ab 53:18 im Tutorial-Video)
   - `git add .`
   - `git commit`
   - Zurück zu Schritt 6
