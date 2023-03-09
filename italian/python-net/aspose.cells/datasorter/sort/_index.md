---
title: metodo sort
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/datasorter/sort/
is_root: false
---
##  sort() {#}
Ordina i dati nell'intervallo.


###  ritorna

gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate.
Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.


```python
def sort(self):
    ...
```




##  sort(cells, area) {#Cells-CellArea}
Ordina i dati della zona.


###  ritorna

gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate.
Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.


```python
def sort(self, cells, area):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| cells | [Cells](/cells/it/python-net/aspose.cells/cells) | Le celle contengono l'area dati.|
| area | [CellArea](/cells/it/python-net/aspose.cells/cellarea) | L'area necessaria per ordinare|


##  sort(cells, start_row, start_column, end_row, end_column) {#Cells-int-int-int-int}
Ordina i dati dell'area.


###  ritorna

gli indici originali (posizione assoluta, ad esempio, la colonna A è 0, B è 1, ...) delle righe/colonne ordinate.
Se nessuna riga/colonna deve essere spostata da questa operazione di ordinamento, verrà restituito null.


```python
def sort(self, cells, start_row, start_column, end_row, end_column):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| cells | [Cells](/cells/it/python-net/aspose.cells/cells) | Le celle contengono l'area dati.|
| start_row | int | La riga iniziale dell'area.|
| start_column | int | La colonna iniziale dell'area.|
| end_row | int | L'ultima fila dell'area.|
| end_column | int | La colonna finale dell'area.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [DataSorter](/cells/it/python-net/aspose.cells/datasorter)
