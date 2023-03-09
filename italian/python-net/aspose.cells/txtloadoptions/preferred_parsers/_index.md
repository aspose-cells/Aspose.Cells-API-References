---
title: preferred_parsers proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 300
url: /it/python-net/aspose.cells/txtloadoptions/preferred_parsers/
is_root: false
---
##  preferred_parsers proprietà

Ottiene e imposta i parser di valori preferiti per il caricamento del file di testo.

###  Osservazioni

parser[0] è il parser che verrà utilizzato per la prima colonna nel file modello di testo,
parser[1] è il parser che verrà utilizzato per la seconda colonna, ...ecc.
L'ultimo (parsers[parsers.length-1]) verrà utilizzato per tutte le altre colonne a partire da parsers.length-1.
Se un elemento è nullo, la colonna corrispondente verrà analizzata dal parser predefinito di Aspose.Cells.
###  Definizione:
```python
@property
def preferred_parsers(self):
    ...
@preferred_parsers.setter
def preferred_parsers(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [TxtLoadOptions](/cells/it/python-net/aspose.cells/txtloadoptions)
