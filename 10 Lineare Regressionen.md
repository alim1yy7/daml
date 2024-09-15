### 46. Beschreiben Sie mindestens drei Gütemaße für Vorhersagequalität von linearen Regressionen
- MAE (Mean Absolute Error): zeigt, um wie viel die Vorhersagen von den tatsächlichen Werten abweichen, Robust gegenüber dem Mean Squared Error (MSE), da keine Fehler quadriert werden
- MSE (Mean Squared Error) ist ähnlich wie der MAE, allerdings werden Fehler hier stärker betont, gut für Modelle, wo Fehler besonders vermieden werden sollen. !!Einheit quadriert!!
- RMSE (Root-MSE), wie MSE, bessere Vergleichbarkeit, da selbe Einheit wie Zielvariable

### 47. Wenn ein lineares Regressionsmodell für Hauspreise zwischen 100k € und 1 Mio. € berechnet wurde, was können Sie dann erwarten von einer Vorhersage für einen Hauspreis von 100 Mio. €?
- Vorhersage liegt weit außerhalb des Trainingsbereichs
- Modell nimmt an, dass die Beziehung zwischen Merkmalen und Preisen linear ist ->extrem hohe oder niedrige Vorhersage

### 48. Wenn Sie eine neue unabhängige Variable bilden, wie Gesamtzeit=Arbeitszeit + Freizeit, was müssen dann machen, um Kollinearität zu vermeiden?
- Entweder eine oder beide alten Variablen aus dem Modell entfernen
- mit VIF auf tatsächliche Kollinearität prüfen


### 49. Warum ist ein one hot encoding mit Weglassen einer Merkmalsausprägung für ein Modell der linearen Regression wichtig?
- **Vermeidung von Multikollinearität**: Durch das Weglassen einer Merkmalsausprägung wird verhindert, dass das Modell überflüssige Information lernt, was zu mathematischen Problemen führt
- Eine Variable erklärt sich durch 2 andere