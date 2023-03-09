---
title: metodo subtotal
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 920
url: /it/python-net/aspose.cells/cells/subtotal/
is_root: false
---
##  subtotal(ca, group_by, function, total_list) {#CellArea-int-ConsolidationFunction-list}
Crea subtotali per l'intervallo.



```python
def subtotal(self, ca, group_by, function, total_list):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| ca | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | La gamma|
| group_by | int | Il campo in base al quale eseguire il raggruppamento, come offset di un numero intero in base zero|
| function | [ConsolidationFunction](/cells/it/python-net/aspose.cells/consolidationfunction) | La funzione del subtotale.|
| total_list | list | Una matrice di offset di campo in base zero, che indica i campi a cui vengono aggiunti i subtotali.|


##  subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data) {#CellArea-int-ConsolidationFunction-list-bool-bool-bool}
Crea subtotali per l'intervallo.



```python
def subtotal(self, ca, group_by, function, total_list, replace, page_breaks, summary_below_data):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| ca | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | La gamma|
| group_by | int | Il campo in base al quale eseguire il raggruppamento, come offset di un numero intero in base zero|
| function | [ConsolidationFunction](/cells/it/python-net/aspose.cells/consolidationfunction) | La funzione del subtotale.|
| total_list | list | Una matrice di offset di campo in base zero, che indica i campi a cui vengono aggiunti i subtotali.|
| replace | bool | Indica se sostituire i subtotali correnti|
| page_breaks | bool | Indica se aggiungere un'interruzione di pagina tra i gruppi|
| summary_below_data | bool | Indica se aggiungere un riepilogo sotto i dati.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
