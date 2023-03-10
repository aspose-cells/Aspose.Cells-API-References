---
title: metodo on_circular
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Implementare questo metodo per fare affari quando si calcolano formule con riferimenti circolari.


###  ritorna

Indica se il motore delle formule deve calcolare tali celle in forma circolare dopo questa chiamata.
True per consentire al motore delle formule di continuare a eseguire i calcoli per loro.
Falso per consentire al motore delle formule di contrassegnare solo quelle celle come Calcolate.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | IEnumerator con elementi CalculationCell che rappresentano celle che<br/> dipendono dai riferimenti circolari.|
###  Osservazioni

Nell'implementazione l'utente può anche impostare il valore previsto come risultato calcolato
per parte/tutte quelle celle in modo che il motore delle formule non le calcoli in modo ricorsivo.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [AbstractCalculationMonitor](/cells/it/python-net/aspose.cells/abstractcalculationmonitor)
