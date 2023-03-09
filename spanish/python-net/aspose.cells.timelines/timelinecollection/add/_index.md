---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos


###  Devoluciones

El nuevo índice de la línea de tiempo add


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| dest_cell_name | str | El nombre de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| base_field_name | str | El nombre de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos


###  Devoluciones

El nuevo índice de la línea de tiempo add


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| dest_cell_name | str | El nombre de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| base_field_index | int | El índice de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos


###  Devoluciones

El nuevo índice de la línea de tiempo add


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| dest_cell_name | str | El nombre de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| base_field | aspose.cells.pivot.PivotField | El PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos


###  Devoluciones

El nuevo índice de la línea de tiempo add


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| base_field_name | str | El nombre de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos


###  Devoluciones

El nuevo índice de la línea de tiempo add


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| base_field_index | int | El índice de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos


###  Devoluciones

El nuevo índice de la línea de tiempo add


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de la línea de tiempo.|
| base_field | aspose.cells.pivot.PivotField | El PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



###  Ver también
* módulo [aspose.cells.timelines](../../)
* clase [TimelineCollection](/cells/es/python-net/aspose.cells.timelines/timelinecollection)
