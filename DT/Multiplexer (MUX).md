- $2^n$-zu-$1$ Bauteil
	- $n-1$ Steuereingänge und $2^n$ Eingänge
- Steuereingänge bestimmen welcher Eingang durchgeleitet wird

### Tabelle (Minimierung)
cb | 00 | 01 | 10 | 11
---|----|----|----|----
a = 0 | 0 | 1 | 1 | 0
a = 1 | 0 | 0 | 1 | 1   
Eingang| 0 | $\bar{a}$ | 1 | $a$

### Bedeutung
- Steuereingänge: c und b
- Eingänge noch abhängig von a
-> Kleiner

### Funktionen auslesen
- Für jede Steuermöglichkeit: was muss anliegen, damit $1$ rauskommt?
- Bei mehreren MUX in Reihe einfach die Klausur verlassen

# Demultiplexer (DX)
- n Steuereingänge, $2^n$ Ausgänge, ein Eingang
- Bei Anliegen von Steuereingängen $abc$ wird der Eingang an den $dec(abc)$-ten Ausgang geleitet
	- MINTerme können verodert werden -> einfache Realisierung von Funktionen!

> [!NOTE]
> $G\frac{0}{2^n - 1}$ entspricht bei MUX/DX den Steuermöglichkeiten (und steht bei den Steuereingängen).

