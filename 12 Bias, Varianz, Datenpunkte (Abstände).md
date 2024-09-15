
Bias = Underfitting (voreingenommen) -> Misst, wie gut das Modell im Durchschnitt die **wahre Beziehung** zwischen Eingabe- und Ausgabevariablen erfasst

Varianz = Overfitting 

### 55. Nennen Sie ein Beispiel für ein überangepasstes Modell (Overfitting)

- Messfehler in Sensoren werden gelernt
### 56. Nennen Sie ein Beispiel für ein unterangepasstes Modell (Underfitting)
- Gewehrschießen mit verbogenem Lauf oder Seitenwind

### 57. Warum wird in einem komplexen Modell (wie Regression mit Polynomen vierten Grades oder Künstliche Neuronale Netze mit sehr vielen Neuronen), der Fehler durch den Bias kleiner?
- Modell hat mehr Kapazität, um komplexe Beziehungen in den Daten zu erkennen
- Bei linearer Regression ist der Bias im Gegesatz umsogrößer

### 58. Skizzieren Sie drei wichtige Abstandsmaße für zwei Datenpunkte in der Fläche. Aus der Skizze muss hervorgeben, welche Abstandsmaße welchen Zeichnungsteilen entsprechen
![[Pasted image 20240915184157.png]]

### 59. Wie werden sich kürzeste und längste Distanz zwischen Datenpunkte bei fortschreitend höheren Dimensionszahl entwicklen? Welcher Art von Bias leigt dem zugrunde?
- **Abstände wachsen insgesamt**: Alle Punkte scheinen weiter auseinander zu liegen.
- **Kürzeste und längste Distanzen nähern sich an**: Unterschied zwischen nah und fern wird kleiner.
- **Fluch der Dimensionalität**: Distanzmaße verlieren an Bedeutung, weil Unterschiede zwischen Distanzen immer geringer werden.
- **Bias**: Distanzen werden weniger nützlich, um echte Unterschiede zu erkennen.

### 60. Welchen Vorteil bieten Spiderdiagramme?
- mehrere Dimensionen, jede Achse 1 Dim.

### 61. Wie können Sie in einen zweidimensionalen Streudiagramm weitere Dimensionen (Variablen) darstellen? Geben Sie je ein Beispiel für die Darstellung einer dritten und vierten Variable
- unterschiedl. Größe der Punkte
- verschiedene Farben