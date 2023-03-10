---
title: metodo find_formula_contains
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 310
url: /it/python-net/aspose.cells/cells/find_formula_contains/
is_root: false
---
##  find_formula_contains(formula, previous_cell) {#str-Cell}
Trova la cella con la formula che contiene la stringa di input.


###  ritorna

Cell oggetto.


```python
def find_formula_contains(self, formula, previous_cell):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| formula | str | La formula da cercare.|
| previous_cell | [Cell](/cells/it/python-net/aspose.cells/cell) |Cella precedente con la stessa formula. Questo parametro può essere impostato su null se si esegue la ricerca dall'inizio.|
###  Osservazioni

Restituisce null (Niente) se non viene trovata alcuna cella.
 NOTA: questo membro è ora obsoleto. Invece,
utilizzare il metodo Cells.Find(object,Cell,FindOptions) con LookInType come LookInType.OnlyFormulas
 e LookAtType come LookAtType.Contains.
 Questo membro verrà rimosso 12 mesi dopo da novembre 2018.
Aspose si scusa per gli eventuali disagi causati.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
