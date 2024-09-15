### 30. Beschreiben Sie kurz zwei Methoden, um kategoriale Variablen als Zahlen aufzubereiten?
- One Hot Encoding (Kodierung von Worten in Binäre Zahlenschreibweise)
- Label-Encoding (Wörtern werden Zahlen zugeordnet)

### 31. Warum sollten Sie für eine mathematische Modellbildung kategoriale Variablen als Zahlen aufbereiten?
- Weil viele numerische Modelle nur mit numerischen Werten arbeiten können

### 32. Was verstehen Sie unter einem [[Daten (Transformierung, Eigenschaften)#One Hot Encoding  |One Hot Encoding]] Trap? Welche Klasse von Modellen ist warum betroffen? Wie werden Sie die neu gebildeten Variablen behandeln, um die Voraussetzungen für die Modellbildung zu erfüllen?

Ein **One-Hot Encoding Trap** tritt auf, wenn bei der Verwendung von One-Hot Encoding für kategorische Variablen in einem linearen Modell alle Dummy-Variablen einbezogen werden, was zu Mehrfachkollinearität führt. Dies geschieht, weil die Dummy-Variablen perfekt korreliert sind. Betroffen sind insbesondere **lineare Modelle** (wie lineare Regression), die Annahmen über die Unabhängigkeit der Variablen machen.

|      | -       | +     |
| ---- | ------- | ----- |
| Rot  | `1 0 0` | `1 0` |
| Grün | `0 1 0` | `0 1` |
| Blau | `0 0 1` | `0 0` |

Um dies zu vermeiden, sollte man eine Dummy-Variable weglassen und die verbleibenden Variablen als Repräsentanten der Kategorien verwenden.

Definition: Einführung einer linearen Abhhängigkeit einer Variablen von der Summe aller anderen Variablen. Betroffen sind alle Regressionsmodelle. Die weggelassene Variable ist aus der Summe - alle anderen berechenbar



### 33. Was werden Sie mit einer Variablen in der Datenaufbereitung machen, die nur einen, immer gleichen Wert in allen Datensätzen enthält?

- Die Variablen zu einer Konstanten machen
- (oder entfernen, da nicht relevant?)

### 34. Was werden Sie mit einer Variablen in der Datenaufbereitung machen, bei der 99% der Datensätzen fehlende Werte haben? Gibt es Ausnahmen zu dieser Regel?
- Datensätze mit so vielen fehlenden Daten werden als nicht relevant angesehen
- Ausnahme, wenn die verbleibenden 1% einen entscheidenden Informationsgehalt besitzen

### 35. Nennen Sie mindestens vier Methoden, um fehlende Werte einer Variablen zu behandeln
- Ersetzen durch Standardwert
- Ersetzen durch Arithmetisches Mittel / Median / Modus
- Durch vorherige oder nachfolgende Werte ersetzen
- Verwenden von statistischen oder Machine Learning-Modellen zur Vorhersage (Regressionsmodell)

### 36. In welchen Kategorie der [[Daten (Transformierung, Eigenschaften)#Missing Values |Missing Values]] (MCAR (missing completely at random), MAR (missing at random), NMAR (not missing at random)) ordnen Sie eine Variable zum Alter von Personen ein, wenn ältere Frauen ihr Alter auslassen und warum?

- NMAR
- Weil das Auslassen direkt mit der Variable "Alter" zusammenhängt

### 37. Wie können Sie mit Lagemaßen Ausreißer einer Variablen erkennen? Nennen Sie mindestens zwei Lagemaße

- Standardabweichung
- Mittelwert
- Korrelationskoeffizient
-

### 38. Erklären Sie den Unterschied zwischen natürlichen und künstlichen Ausreißern
- natürliche Ausreißer sind seltene Ereignisse wie das Auftreten einer neuen Kundengruppe, Naturereignisse, Streiks, regulatorische Eingriffe
- Künstiliche Ausreiißer sind Fehler im Rahmen von Datenerhebung (Messfehler, fehlerhafte Codierung (Euro und Tausender Euro) und fehlerhafte Datenzusammenführung)

### 39. Warum ist eine Standardisierung der Variablen wichtig?

- Um eine Vergleichbarkeit von Variablen sicherzustellen
- Erleichtert die Interpretation