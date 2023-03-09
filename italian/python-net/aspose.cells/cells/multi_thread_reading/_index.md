---
title: multi_thread_reading proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1200
url: /it/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading proprietà

Ottiene o imposta se il modello di dati delle celle deve supportare la lettura multithread.
Il valore predefinito di questa proprietà è false.

###  Osservazioni

Se sono presenti più thread per leggere contemporaneamente gli oggetti Row/Cell in questa raccolta,
questa proprietà dovrebbe essere impostata come true, altrimenti potrebbero essere prodotti risultati imprevisti.
Il supporto della lettura multithread può ridurre le prestazioni per l'accesso agli oggetti Row/Cell da questa raccolta.
Si prega di notare che alcune funzionalità non possono supportare la lettura multi-thread,
come i valori di formattazione (di [Cell.string_value](/cells/it/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/it/python-net/aspose.cells/cell#display_string_value), .etc.).
Pertanto, anche con questa proprietà impostata su true, tali API potrebbero comunque fornire risultati imprevisti per la lettura multithread.
###  Definizione:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
