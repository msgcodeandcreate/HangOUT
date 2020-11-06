# HangOUT
Tools zur Kommunikation zwischen Kolleginnen und Kollegen im Homeoffice


## Die Idee
Entwicklung eines Tools zur Kommunikation zwischen Kolleginnen und Kollegen im Homeoffice



## Anfängliche Planung

### Schritt 1: Szenario:
Ihre Freunde kommen zu Ihnen und bitten Sie, einen Turnier-Tracker zu erstellen. Sie spielen ständig Spiele und wollen herausfinden, wer der Beste ist.
Die Idee besteht darin, dass Sie ein Bracket-Turniersystem erstellen, bei dem der Computer ihnen sagt, wer in einem Bracket im Einzelausscheidungsstil spielen soll. Am Ende soll der Sieger ermittelt werden. Ihr Modell ist die NCAA-Basketball-Turnierrunde für March Madness.

## Anforderungen
* Audio-und Videoübertragung
* Chatfunktion
* Gruppen-und Privatunterhaltungen
* Räume zum Betreten und Verlassen, Pausenraum, Projektraum
* Minispiele: Tic TacToe; Schnick, Schnack, Schnuck; „Wer bin ich?“, Schach, Hangman, Extra Fenster: Frage stellen und Punkte sammeln für erste richtige Antwort
* Räume reservieren können, Besetzzeichen

### Schritt 2: Fragen (Für weitere Anforderungsspezifikation)
Wie viele Spielerinnen und Spieler wird das Turnier behandeln? ist es variabel?
Die Anwendung sollte in der Lage sein

Wie gehen wir damit um, wenn ein Turnier weniger als die volle Anzahl von Spielern hat?
Sollte die Reihenfolge, wer gegeneinander spielt, zufällig oder nach der Reihenfolge der Eingaben geordnet sein?
Sollen wir das Spiel planen oder werden sie nur wann immer gespielt?
Wenn die Spiele geplant sind, woher weiß das System, wann die Spiele anzusetzen sind?
Wenn die Spiele wann immer gespielt werden, kann dann ein Spiel aus der zweiten Runde gespielt werden, bevor die erste Runde beendet ist?
Muss das System eine Art Punktestand speichern oder nur, wer gewonnen hat?
Welche Art von Front-End sollte dieses System haben (winform, Webpage, App. etc.)?
Wo sollen die Daten gespeichert werden?
Wird dieses System Anmeldegebühren, Preise oder andere Auszahlungen verwalten?
Welche Art von Berichterstattung ist erforderlich?
Wer kann die Ergebnisse eines Spiels ausfüllen?
Gibt es unterschiedliche Zugangsebenen?
Soll dieses System die BenutzerInnen über bevorstehende Spiele informieren?
Ist jeder Spieler auf sich allein gestellt oder können Teams diesen Turnier-Tracker benutzen?



## Schlüsselbegriffe
E-Mail
SQL
Benutzerdefinierte Ereignisse
Fehlerbehandlung
Schnittstellen
Zufällige Anordnung
Texterstellung
    
Schritt 3: Datenentwurf
Kartierung der Daten
Mannschaft
Teammitglieder (Liste<Person>
TeamName (Zeichenfolge)

## Person 
Vorname (Zeichenfolge)
Nachname (Zeichenfolge)
E-Mail-Adresse (Zeichenfolge)
Handynummer (Zeichenfolge)

Turnier
TurnierName (Zeichenfolge)
EntryFee (dezimal)
EingetrageneTeams (Liste<Team>)
Preise (Liste<Preis>)
Runden (Liste<Liste<Abgleich>>)  

Preis
OrtNummer (int)
Ortsname (Zeichenfolge)
PreisBetrag (dezimal)
PreisProzentsatz (doppelt)

Vergleich
Einträge (Liste<Matchup-Eintrag>)
Sieger (Mannschaft)
MatchupRunde (int)

MatchupEintrag
TeamWettbewerb (Mannschaft)
Punktzahl (doppelt)
ParentMatchup (Abgleich)

## Benutzeroberflächen-Design
### Haupt-Viewer


