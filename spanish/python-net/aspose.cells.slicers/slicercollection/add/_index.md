---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.slicers/slicercollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
Agregue un nuevo Slicer usando PivotTable como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango Slicer.|
| base_field_name | str | El nombre de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

slicers.add(pivot, "E3", "fruit")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
Agregue un nuevo Slicer usando PivotTable como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango Slicer.|
| base_field_index | int | El índice de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

slicers.add(pivot, "E20", 0)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
Agregue un nuevo Slicer usando PivotTable como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango Slicer.|
| base_field | aspose.cells.pivot.PivotField | El PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

slicers.add(pivot, "I3", pivot.base_fields[0])

```


##  add(table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-str}
Agregue un nuevo Slicer usando ListObjet como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, table, index, dest_cell_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | objeto ListObject|
| index | int | El índice de ListColumn en ListObject.ListColumns|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango Slicer.|

###  Ejemplos

```python

slicers.add(table, 1, "E38")

```


##  add(table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str}
Agregue un nuevo Slicer usando ListObjet como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, table, list_column, dest_cell_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | objeto ListObject|
| list_column | aspose.cells.tables.ListColumn | ListColumn en ListObject.ListColumns|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango Slicer.|

###  Ejemplos

```python

slicers.add(table, table.list_columns[1], "I38")

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
Agregue un nuevo Slicer usando PivotTable como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer.|
| base_field_name | str | El nombre de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

slicers.add(pivot, 20, 12, "fruit")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
Agregue un nuevo Slicer usando PivotTable como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer.|
| base_field_index | int | El índice de PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

slicers.add(pivot, 20, 8, 0)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
Agregue un nuevo Slicer usando PivotTable como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, pivot, row, column, base_field):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |Objeto de tabla dinámica|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer.|
| base_field | aspose.cells.pivot.PivotField | El PivotField en PivotTable.BaseFields|

###  Ejemplos

```python

slicers.add(pivot, 3, 12, pivot.base_fields[0])

```


##  add(table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
Agregue un nuevo Slicer usando ListObjet como fuente de datos


###  Devoluciones

El nuevo índice add Slicer


```python
def add(self, table, list_column, row, column):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject | objeto ListObject|
| list_column | aspose.cells.tables.ListColumn | ListColumn en ListObject.ListColumns|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer.|

###  Ejemplos

```python

slicers.add(table, table.list_columns[1], 38, 12)

```



###  Ver también
* módulo [aspose.cells.slicers](../../)
* clase [SlicerCollection](/cells/es/python-net/aspose.cells.slicers/slicercollection)
