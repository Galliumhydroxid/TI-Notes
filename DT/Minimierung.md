## Definitionen
- Disjunktive Normalform: Disjunktion von Konjunktivtermen
	- "Alle erfüllenden Terme verodern"
- Konjunktive Normalform: Konjunktion von Disjunktivtermen
	- "Alle _nicht_ erfüllenden Terme negieren, und verunden"
- MINterme / MAXterme: Terme der DNF/KNF

## Shannonscher Entwicklungssatz
![[Pasted image 20230323214113.png]]


## KV-Minimierung
- Aus KNF/DNF trivial
	- In die Zellen die Funktionswerte
- Implikant: und-Verknüpfung von Einsen im Diagramm
- Prim-Implikant: Implikant, welcher aus keinem anderen folgt
- Kern-Prim-Implikant: Prim-Implikant, welcher einen Minterm überdeckt, welcher von keinem anderen Primimplikanten überdeckt wird
- Minimalform: die Überdeckung aus möglichst großen Teilen (mögl. kleinen Termen)

## Quine-McCluskey

![[Pasted image 20230321143030.png]]
### O. Ordnung
- Alle MINterme untereinander
	- Gruppiere die Terme nach der Anzahl der Einsen
### n+1. Ordnung
- Fasse immer die Terme zusammen, die sich in genau einer Variable unterscheiden
- Schreibe diese als "Don't-Care"
- Don't-Care-Stellen müssen auch an den gleichen Stellen sein!
### Abbruchbedingung
- Wenn sich keine Terme mehr zusammenfassen lassen
- Markiere die **Primimplikanten** mit A, B, ...

### 2. Quinesche Tabelle
![[Pasted image 20230321144134.png]]
- Alle Primimplikanten, welche alleinig für einen Term verantwortlich sind, sind Kernprimimplikanten

## Consensus
![[Pasted image 20230321145840.png]]
