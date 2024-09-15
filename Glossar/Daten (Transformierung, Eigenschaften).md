### Data-Pipelines
Data Pipelines sind automatisierte Systeme, die den Prozess des Sammelns, Verarbeitens und Speicherns von Daten von der Quelle bis zur Zielanwendung steuern. Sie sorgen dafür, dass Daten in einem strukturierten und effizienten Fluss durch verschiedene Phasen der Verarbeitung laufen.

**Kernpunkte:**

- **Datenfluss**: Sie definieren die Route und die Schritte, die Daten durchlaufen.
- **Automatisierung**: Sie automatisieren die Schritte der Datenverarbeitung, ohne manuelles Eingreifen.
- **Stufen**: Typische Phasen sind Extraktion (Datenabholung), Transformation (Datenaufbereitung) und Laden (Speichern der Daten).

**Beispiel**: Eine Pipeline könnte Daten aus einer SQL-Datenbank extrahieren, sie in ein Analyseformat transformieren und dann in ein Data Warehouse laden.

# Univariate Daten
- Beziehen sich auf ein einziges Merkmal
# Bivariate Daten
- Daten zu jeder von zwei Variablen
- Analyse, ob 2 Daten miteinander in Verbindung stehen
- **Beispiel**: Die Beziehung zwischen der Anzahl der Studienstunden (Variable 1) und den Prüfungsnoten (Variable 2) oder die Verbindung zwischen dem Einkommen und der Ausgabenhöhe.

### One Hot Encoding
One Hot Encoding ist ein Verfahren, um kategorische (nominale, ordinale) Daten in numerische Daten zu transformieren. Dieses Verfahren findet während des Pre-Processings statt.

### Missing Values
| **Kategorie** | **Definition**                                                                                   | **Beispiel**                                                                                          | **Behandlung**                                                       |
| ------------- | ------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| MCAR          | Fehlende Werte sind völlig zufällig und unabhängig von anderen Variablen.                        | Ein Umfrageteilnehmer überspringt zufällig eine Frage.                                                | Relativ einfach zu handhaben, da keine Verzerrung.                   |
| MAR           | Fehlende Werte hängen von beobachteten Variablen ab, aber nicht von den fehlenden Werten selbst. | z.B.  Frauen geben seltener ihr Alter an, aber das Fehlen ist nicht direkt vom Alter selbst abhängig. | Imputation durch Modelle, die beobachtete Variablen berücksichtigen. |
| NMAR          | Fehlende Werte sind direkt abhängig von den fehlenden Werten selbst.                             | Ältere Menschen geben ihr Alter nicht an, weil sie sich unwohl fühlen, ihr Alter preiszugeben.        | Spezialmethoden erforderlich, z.B. Modelle für NMAR-Daten.           |
### Standardisierung der unabhängigen Variablen
- **Transformation** der Variablen, sodass sie einen **einheitlichen Maßstab** haben.
- Typischerweise: **Mittelwert = 0** und **Standardabweichung = 1**.
- Ziel: **Vergleichbarkeit** der Variablen und Verbesserung der **Modellleistung**