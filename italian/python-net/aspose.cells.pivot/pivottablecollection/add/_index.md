---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.


###  ritorna

Il nuovo indice della cache aggiunto.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_data | str | I dati per la nuova cache della tabella pivot.|
| dest_cell_name | str |La cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot.


###  ritorna

Il nuovo indice di tabella pivot aggiunto.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/it/python-net/aspose.cells.pivot/pivottable) | La tabella pivot di origine.|
| dest_cell_name | str |La cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.


###  ritorna

Il nuovo indice della cache aggiunto.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_data | str | I dati per la nuova cache della tabella pivot.|
| dest_cell_name | str |La cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|
| use_same_source | bool | Indica se utilizzare la stessa origine dati quando un'altra tabella pivot esistente ha utilizzato questa origine dati.<br/> Se la proprietà è true, salverà la memoria.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.


###  ritorna

Il nuovo indice della cache aggiunto.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_data | str | L'intervallo di celle di dati per la nuova tabella pivot.Esempio: Sheet1!A1:C8|
| row | int | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| column | int | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot.


###  ritorna

Il nuovo indice di tabella pivot aggiunto.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/it/python-net/aspose.cells.pivot/pivottable) | La tabella pivot di origine.|
| row | int | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| column | int | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
Aggiunge una nuova cache della tabella pivot a una raccolta PivotCaches.


###  ritorna

Il nuovo indice della cache aggiunto.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_data | str | L'intervallo di celle di dati per la nuova tabella pivot.Esempio: Sheet1!A1:C8|
| row | int | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| column | int | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|
| use_same_source | bool | Indica se utilizzare la stessa origine dati quando un'altra tabella pivot esistente ha utilizzato questa origine dati.<br/> Se la proprietà è true, salverà la memoria.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati.


###  ritorna

Il nuovo indice di tabella pivot aggiunto.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_data | list | Gli intervalli di consolidamento multipli, ad esempio {"Foglio1!A1:C8","Foglio2!A1:B8"} |
| is_auto_page | bool | Se creare automaticamente un campo a pagina singola.<br/>Se vero, il seguente parametro pageFields verrà ignorato.|
| page_fields | [PivotPageFields](/cells/it/python-net/aspose.cells.pivot/pivotpagefields) | Gli elementi del campo della pagina pivot.|
| dest_cell_name | str | destCellName Il nome del nuovo rapporto di tabella pivot.|
| table_name | str | il nome del nuovo rapporto di tabella pivot.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati.


###  ritorna

Il nuovo indice di tabella pivot aggiunto.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| source_data | list | Gli intervalli di consolidamento multipli, ad esempio {"Foglio1!A1:C8","Foglio2!A1:B8"} |
| is_auto_page | bool | Se creare automaticamente un campo a pagina singola.<br/> Se vero, il seguente parametro pageFields verrà ignorato|
| page_fields | [PivotPageFields](/cells/it/python-net/aspose.cells.pivot/pivotpagefields) | Gli elementi del campo della pagina pivot.|
| row | int | Indice di riga della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| column | int | Indice di colonna della cella nell'angolo superiore sinistro dell'intervallo di destinazione del rapporto di tabella pivot.|
| table_name | str | Il nome del nuovo rapporto di tabella pivot.|



###  Guarda anche
* modulo [aspose.cells.pivot](../../)
* classe [PivotTableCollection](/cells/it/python-net/aspose.cells.pivot/pivottablecollection)
