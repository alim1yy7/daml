### 62. Welche mindestens drei Hyperparameter sind für das k-nächste Nachbarn Verfahren wichtig?
- Gewichtung der Nachbarn
- Anzahl der Nachbarn k für eine Mehrheitsentscheidung
- Abstandsmaß / Distanzmetrik (Euclidean Distance, Manhattan Distance)

### 63. Warum wird meistens eine ungerade Anzahl Nachbarn im k-nächste Nachbarn Verfahren für die Mehrheitsbestimmung einer Vorhersage verwendet?
- Da eine Mehrheitsentscheidung notwendig ist

### 64. Warum zählen Sie das k-NN Verfahren zum überwachten oder zum nicht überwachten Lernen?
- Überwachtes Lernen, da Labels bekannt sind

### 65. Warum müssen im k-Nächste Nachbarn Verfahren die unabhängigen Variablen auf eine gemeinsame Skala gebracht werden?
- Damit die Distanzen nicht verzerrt werden

### 66. Wenn im k-nächste Nachbarn Verfahren k=1 gesetzt wird, tritt dann Über- oder Unteranpassung auf? Wird die Varianz der Schätzung auf den Testdaten dann hoch oder niedrig sein?
- Überanpassung
- Hohe Varianz

### 67. Warum ist für das k-Nächste Nachbarn Verfahren streng genommen keine Modellbildung erforderlich? Wie wird im Englischen ein derartiges Lernverfahren genannt?
- Vorhersagen werden erst **im Moment der Abfrage** (also beim Testen) getroffen, indem die **k nächsten Nachbarn** eines neuen Datenpunkts aus den Trainingsdaten gesucht werden.
- Lazy-Learning-Verfahren