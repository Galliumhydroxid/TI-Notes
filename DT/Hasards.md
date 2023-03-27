- Statische Übergänge: Ausgangsbelegung bleibt am Anfang und Ende gleich, ändert sich aber zwischendurch
- Dynamische Übergänge: Ausgangsbelegung verändert sich, und "jittert" dazwischen zusätzlich

# Totzeiten
- Totzeiten von Variablen: Pfad von hinten nach vorne verfolgen und zusammenzählen
	- bei mehreren Möglichkeiten: trotzdem verfolgen, und am Anfang zusammenführen

# Definitionen
- Hasard: Vorbedingung von einem Hasardfehler
- Hasardfehler: ...
- Funktionshasard: ein in der Funktion intrinsischer Hasard
	- Kann **nicht** behoben werden!
	- Hasardfehler kann durch Verzögerungen vermieden werden
- Strukturhasard: ein in dem Schaltnetz intrinsischer Hasard
	- Kann in dem Schaltnetz behoben werden

# Beispiel
- Funktionshasard: $\bar{e_1}e_2 \lor e_1 e_3$
	- $(1, 1, 0) \mapsto (1, 0, 1)$
	- KV-Diagramm -> alle möglichen Wege von 6 zu 5
	- Wenn es einen nicht-monotonen Weg gibt, dann gibt es einen Hazard
		- $(1, 1, 0) \mapsto (1, 0, 0) \mapsto (1, 0, 1)$
		- Alarm: $e_2$ nicht monoton! -> Funktionshasard
- Strukturhasard: füge zusätzliche Variablen aus dem Totzeitmodell hinzu
	- $e_{11} \bar{\lor} e_{12}$ nicht möglich -> ausgrauen
	- KV-Diagramm mit zusätzlichen Variablen malen
	- Beispiel von oben: $12 \mapsto 13 \mapsto 15$ ist nicht monoton in $e_{11}$ 
		- Strukturhasard!
- Tritt ein Hasardfehler ein?
	- Zeitdiagramm malen, auf "Jitter" im Ausgang achten