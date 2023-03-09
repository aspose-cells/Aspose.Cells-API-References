---
title: metodo delete_rows
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 260
url: /it/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
Elimina diverse righe.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| row_index | int |L'indice della prima riga da eliminare.|
| total_rows | int | Numero di righe da eliminare.|
###  Osservazioni

Se l'intervallo eliminato contiene la parte superiore (non intera) della tabella (ListObject),
non è stato possibile eliminare l'intervallo e non verrà fatto nulla. Funziona come MS Excel.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
Elimina più righe nel foglio di lavoro.


###  ritorna




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| row_index | int | Indice di riga.|
| total_rows | int | Numero di righe da eliminare.|
| update_reference | bool | Indica se aggiornare i riferimenti in altri fogli di lavoro.|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
