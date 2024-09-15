Siehe [[Bilder#! Pasted image 20240915173958.png|Wahrheitsmatrix]]
### 50. Was sind umgangssprachlich falsch positive Vorhersagen (FP)? Geben Sie mindestens ein Beispiel
- Modell zeigt fälschlicherweise ein positives Ergebnis, obwohl es in Wirklichkeit nicht eingetreten ist
- **Beispiel:** Ein Corona-Schnelltest zeigt ein positives Ergebnis, obwohl der Patient eigentlich negativ ist
  - Fehlalarm

### 51. Was sind umgangssprachlich falsch negative Vorhersagen (FN)? Geben Sie mindestens ein Beispiel
- Modell zeigt fälschlicherweise ein negatives Ergebnis, obwohl es in Wirklichkeit positiv wäre
- **Beispiel:** Spam-Filter erkennt Spam-Email nicht und zeigt diese im Postfach an
- Blindgänger

### 52. Beschreiben Sie verbal oder als Formel  das Modellgütemaß der Genauigkeit für eine binäre Klassifikation mit den Begriffen von True Positive (TP), False Positive (FP), True Negative (TN), False Negative (FN) für die Ergebnisse der Klassifikation
- Genauigkeit misst den Anteil der korrekt klassifizierten Fälle (TP als auch TN) an allen Vorhersagen

### 53. Ist die Genauigkeit, definiert als (TP+TN) / (TP+TN + FP+FN) ein verlässliches Gütemaß für eine binäre Klassifikation von seltenen Ereignissen? Hier gilt TP True Positive, TN True Negative, FP False Positive, FN False Negative
- Bei einer Krankheit mit einer Prävalenz von 1 % könnte das Modell immer „gesund“ vorhersagen, 99 % Genauigkeit erreichen, aber alle **positiven Fälle verpassen**

### 54. Geben Sie mindestens je ein Beispiel für unterschiedliche Kosten von FP und FN Vorhersagen
- FP: Abschuss eines vermeindlich feindlichen Flugzeugs
- FN: Terrorist gelangt ins Stadion