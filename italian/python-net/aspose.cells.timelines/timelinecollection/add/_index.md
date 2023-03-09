---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati


###  ritorna

Il nuovo indice Timeline add


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | Oggetto tabella pivot|
| dest_cell_name | str | Il nome della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| base_field_name | str | Il nome di PivotField in PivotTable.BaseFields|

###  Esempio

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati


###  ritorna

Il nuovo indice Timeline add


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | Oggetto tabella pivot|
| dest_cell_name | str | Il nome della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| base_field_index | int | L'indice di PivotField in PivotTable.BaseFields|

###  Esempio

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati


###  ritorna

Il nuovo indice Timeline add


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | Oggetto tabella pivot|
| dest_cell_name | str | Il nome della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| base_field | aspose.cells.pivot.PivotField | Il campo pivot in PivotTable.BaseFields|

###  Esempio

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati


###  ritorna

Il nuovo indice Timeline add


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | Oggetto tabella pivot|
| row | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| column | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| base_field_name | str | Il nome di PivotField in PivotTable.BaseFields|

###  Esempio

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati


###  ritorna

Il nuovo indice Timeline add


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | Oggetto tabella pivot|
| row | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| column | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| base_field_index | int | L'indice di PivotField in PivotTable.BaseFields|

###  Esempio

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Aggiungi una nuova sequenza temporale utilizzando la tabella pivot come origine dati


###  ritorna

Il nuovo indice Timeline add


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable | Oggetto tabella pivot|
| row | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| column | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo della sequenza temporale.|
| base_field | aspose.cells.pivot.PivotField | Il campo pivot in PivotTable.BaseFields|

###  Esempio

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



###  Guarda anche
* modulo [aspose.cells.timelines](../../)
* classe [TimelineCollection](/cells/it/python-net/aspose.cells.timelines/timelinecollection)
