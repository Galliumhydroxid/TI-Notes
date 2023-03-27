- Physikalischer Speicher kontinuierlich und stetig
	- Pages haben keinen eigenen adress space
- virtuelle Adresse:  PAGE_NR | OFFSET 
- Pages werden gemapped
# Cache
## Typen
- direct-mapped: hash
- fully-associative: freie Zeilen werden gefüllt
- set-associative: gottlose Mischung
---
- Blockgröße: Offsetaddressierung
- Adresse: TAG | INDEX | OFFSET