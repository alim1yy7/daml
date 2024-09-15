### 40. Warum wird in der deskriptiven Statistik keine Abtrennung von Validierungsdaten angewendet?
- Validierungsdaten werden bei der Modellbildung benötigt
- Deskrti

### 41. Nennen Sie mindestens zwei Methoden der Kreuzvalidierung
1) Leave-One-Out Kreuzvalidierung:
	- Training auf n-1 Datenpunkten
	- Validierung auf 1 Datenpunkt
2) Holdout Method: Ein Teil der Datenmenge wird exklusiv für die Validierung zurück gehalten

### 42. In welchem Fall werden Sie auf die Abtrennung einer eigenen Test- und Validierungsmenge verzichten? Was müssen Sie dann bei der Bestimmung der Modellgüteparameter beachten?
- Wenn Methoden wie die k-Fache Kreuzvalidierung verwendet werden 
- Wenn ein kleiner Datensatz vorliegt -> Der gesamte Datensatz wird für die k-Fache X-Val verwendet
- Gefahr des Overfittings -> Modell zu stark auf Trainingsdaten optimiert

### 43. Warum werden Sie eine k-fache Kreuzvalidierung während des Trainings nicht auf die Testdaten anwenden?
- K-fache Kreuzvalidierung nur für **Trainings- und Validierungsdaten**
- Anwendung auf Testdaten führt zu **Overfitting** und **Daten-Leakage**
- **Testdaten erst nach dem Training** für die finale Leistungsmessung verwenden

### 44. Warum liegt ein unzulässiges Datenleck (Data Leakage) vor, wenn Sie Röntgenaufnahmen zu Knochenbrüchen von 30000  Patienten, jeweils mit 3 Bildern,  untersuchen und die Aufnahmen zufällig auf Trainings- und Testdaten verteilen? Wie müssen Sie die Datenaufteilung richtig machen?
- Mehrere Aufnahmen eines Patienten im Trainings- und Testdatensatz
- Bilder eines Patienten entweder im Training- oder Testdatensatz

### 45. Warum müssen Sie die Parameter (Min, Max, Mittelwert, Standabweichung) für eine [[Daten (Transformierung, Eigenschaften)#Standardisierung der unabhängigen Variablen |Standardisierung der unabhängigen Variablen]] bei einer Modellerstellung nach der Trainings-/Testaufteilung der Daten nur auf den Trainingsdaten berechnen und dann erst auf die Testdaten anwenden?
- **Vermeidung von Daten-Leakage**: Testdaten dürfen nicht ins Training „leaken“.
- Testdaten sollen **ungesehen** bleiben, um die **Generalisierungsleistung** des Modells korrekt zu bewerten.
- Die Berechnung der Standardisierungsparameter auf Testdaten würde das Modell mit **zukünftigen Informationen** versorgen.