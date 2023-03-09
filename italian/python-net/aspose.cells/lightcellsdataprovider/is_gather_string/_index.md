---
title: metodo is_gather_string
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Controlla se il valore di stringa corrente della cella deve essere raccolto in un pool globale.


###  ritorna

true se il valore stringa deve essere raccolto in un pool globale per il file risultante.


```python
def is_gather_string(self):
    ...
```


###  Osservazioni

La raccolta di valori di stringa trarrà vantaggio solo quando sono presenti molti valori di stringa duplicati per le celle fornite da questa implementazione.
In questa situazione la raccolta di stringhe farà risparmiare molta memoria e genererà un file risultante più piccolo.
Se ci sono molti valori stringa per le celle fornite da LightCellsDataProvider ma pochi di essi sono uguali,
la raccolta della stringa costerà più memoria e tempo e non ha alcun vantaggio per il file risultante.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [LightCellsDataProvider](/cells/it/python-net/aspose.cells/lightcellsdataprovider)
