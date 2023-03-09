---
title: metodo get_dependents_in_calculation
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 390
url: /it/python-net/aspose.cells/cells/get_dependents_in_calculation/
is_root: false
---
##  get_dependents_in_calculation(row, column, recursive) {#int-int-bool}
Ottiene tutte le celle il cui risultato calcolato dipende da celle specifiche.


###  ritorna

Enumeratore per enumerare tutti i dipendenti (oggetti Cell)


```python
def get_dependents_in_calculation(self, row, column, recursive):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| row | int | Indice di riga della cella specifica|
| column | int | Indice di colonna della cella specifica.|
| recursive | bool | Se restituisce quei dipendenti che non fanno riferimento direttamente alla cella specifica<br/> ma riferimento ad altre foglie di quella cella.|
###  Osservazioni

Per utilizzare questo metodo, assicurati che la cartella di lavoro sia stata impostata con il valore vero per
[FormulaSettings.enable_calculation_chain](/cells/it/python-net/aspose.cells/formulasettings#enable_calculation_chain) ed è stato interamente calcolato con questa impostazione.
Se non è presente alcun riferimento alla formula per questa cella, verrà restituito null.
Per maggiori dettagli ed esempio, vedere [Cell.get_dependents_in_calculation(recursive)](/cells/it/python-net/aspose.cells/cell/get_dependents_in_calculation)


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
