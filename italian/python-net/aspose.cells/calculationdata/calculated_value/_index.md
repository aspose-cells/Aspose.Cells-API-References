---
title: calculated_value proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 50
url: /it/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
##  calculated_value proprietà

Ottiene o imposta il valore calcolato per questa funzione.

###  Osservazioni

L'utente deve impostare questa proprietà nel suo motore di calcolo personalizzato per le funzioni supportate dal motore,
il valore impostato verrà restituito quando si ottiene questa proprietà in un secondo momento.
Il valore impostato può essere qualsiasi valore di quegli oggetti che possono essere impostati su Cell(Cell.Value).
E può anche essere un array di questo tipo di valori o un intervallo, un nome, un'area di riferimento.
Ottenere questa proprietà prima dell'impostazione farà sì che la funzione venga calcolata dal motore di calcolo predefinito di Aspose.Cells e verrà restituito il valore calcolato.
###  Definizione:
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [CalculationData](/cells/it/python-net/aspose.cells/calculationdata)
