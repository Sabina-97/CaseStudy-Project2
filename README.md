# **PROJECT 2: Indoor Localization**
### Subject: Case Study 1  
### Localization based on Received Signal Strength (RSS), using k-NN

---

## Projektzusammenfassung

Im Rahmen dieses Projekts wurde ein Indoor-Positionierungssystem entwickelt, das auf der Auswertung von WiFi-Signalen basiert. Ziel war es, die Position eines mobilen Geräts innerhalb eines Gebäudes möglichst präzise zu bestimmen, ohne auf zusätzliche Sensorik oder Infrastruktur angewiesen zu sein. Grundlage der Positionsbestimmung bildet ein k-Nearest-Neighbors-Algorithmus (k-NN), der sowohl in gewichteter als auch ungewichteter Form implementiert wurde.

Die verwendeten Daten umfassen RSSI-Messungen (Received Signal Strength Indicator) mehrerer WLAN-Access-Points, welche an verschiedenen Positionen und in unterschiedlichen Ausrichtungen innerhalb eines Gebäudes erfasst wurden. Durch die Vorverarbeitung wurden Offline- und Online-Datensätze erstellt, aus denen charakteristische Merkmale extrahiert wurden. Zur Reduktion von Orientierungsabhängigkeiten wurde ein Parameter *m* eingeführt, der die *m* ähnlichsten Orientierungswinkel pro Referenzpunkt berücksichtigt.

Ein zentraler Bestandteil des Projekts war die systematische Optimierung der Modellparameter *k* (Anzahl der nächsten Nachbarn) und *m* (Anzahl der berücksichtigten Orientierungen) mittels Cross-Validation. Zur Bewertung der Modellgüte wurden Fehlermaße wie der mittlere Positionsfehler und die Root Mean Square Error (RMSE) verwendet. Darüber hinaus wurden verschiedene Visualisierungen – unter anderem Boxplots, Oberflächenplots und Fehlerverteilungen – eingesetzt, um die Leistungsfähigkeit des Systems zu analysieren.

Die Ergebnisse zeigen, dass der gewichtete k-NN-Ansatz im Vergleich zur ungewichteten Variante eine leicht höhere Genauigkeit erreicht. In beiden Fällen konnte eine mittlere Positionsgenauigkeit von unter drei Metern erzielt werden, was für viele Indoor-Navigation-Anwendungen ausreichend ist.

---

## Fazit

Das Projekt demonstriert erfolgreich, dass eine rein signalbasierte Positionsschätzung mit einfachen, aber wirkungsvollen Methoden wie k-NN praktikabel und effektiv realisiert werden kann – auch ohne komplexe Infrastruktur oder zusätzliche Hardware.
