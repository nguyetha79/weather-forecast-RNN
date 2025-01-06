# Wettervorhersage mit RNN
Im Rahmen des Kurses "Grundlagen der Computational Intelligence" habe ich ein Projekt durchgeführt, das zeigt, wie man Recurrent Neural Networks (RNNs) mit Long Short-Term Memory (LSTM)-Einheiten für die Wettervorhersage verwendet, um den Einfluss der Kontextgröße zu untersuchen. Das Notebook `zeitreihenprognose_wettervorhersage.ipynb` umfasst die folgenden wichtigen Schritte:

**1. Datenvorbereitung:**
- Installation der erforderlichen Bibliotheken, einschließlich TensorFlow.
- Laden und Normalisieren des Jena Climate-Datensatzes, der verschiedene Wetterattribute enthält, die alle 10 Minuten aufgezeichnet werden.

**2. Datenvisualisierung:**
- Visualisierung der Rohdaten, um die Muster und Verteilungen der verschiedenen Wettermerkmale zu verstehen.

**3. Datenvorverarbeitung:**
- Down-sampling der Daten, um die Anzahl der Datenpunkte zu reduzieren.
- Normalisierung der ausgewählten Merkmale, um die Eingabewerte zu standardisieren.

**4. Datensatz-Erstellung:**
- Aufteilung der Daten in Trainings- und Validierungssätze.
- Erstellung von Zeitreihendatensätzen mit der Methode timeseries_dataset_from_array von Keras.

**5. Modellaufbau:**:
- Definition der LSTM-Modellarchitektur mit Input-, LSTM- und dense Layers.
- Kompilierung des Modells mit dem Adam-Optimierer und der Mean Squared Error-Verlustfunktion.

**6. Modelltraining:**
- Training des Modells mit den Trainings- und Validierungsdatensätzen.
- Verwendung von Callbacks für frühzeitiges Stoppen und Speichern der besten Modell-Checkpoints.

**7. Auswertung:**
- Bewertung der Modellleistung mit dem Mean Absolute Error (MAE).
