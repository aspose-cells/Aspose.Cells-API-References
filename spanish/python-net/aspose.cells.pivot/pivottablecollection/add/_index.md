---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.


###  Devoluciones

El nuevo índice de caché agregado.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_data | str | Los datos para la nueva caché de tabla dinámica.|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
Agrega un nuevo objeto de tabla dinámica a la colección desde otra tabla dinámica.


###  Devoluciones

El nuevo índice de tabla dinámica agregado.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/es/python-net/aspose.cells.pivot/pivottable) | La tabla dinámica de origen.|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.


###  Devoluciones

El nuevo índice de caché agregado.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_data | str | Los datos para la nueva caché de tabla dinámica.|
| dest_cell_name | str | La celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|
| use_same_source | bool | Indica si se usa la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos.<br/> Si la propiedad es verdadera, ahorrará memoria.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.


###  Devoluciones

El nuevo índice de caché agregado.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_data | str | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1! A1: C8|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
Agrega un nuevo objeto de tabla dinámica a la colección desde otra tabla dinámica.


###  Devoluciones

El nuevo índice de tabla dinámica agregado.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/es/python-net/aspose.cells.pivot/pivottable) | La tabla dinámica de origen.|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.


###  Devoluciones

El nuevo índice de caché agregado.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_data | str | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1! A1: C8|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|
| use_same_source | bool | Indica si se usa la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos.<br/> Si la propiedad es verdadera, ahorrará memoria.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
Agrega un nuevo objeto de tabla dinámica a la colección con varios rangos de consolidación como fuente de datos.


###  Devoluciones

El nuevo índice de tabla dinámica agregado.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_data | list | Los múltiples rangos de consolidación, como {"Hoja1!A1:C8","Hoja2!A1:B8"} |
| is_auto_page | bool | Si crea automáticamente un campo de una sola página.<br/> Si es verdadero, se ignorará el siguiente parámetro pageFields.|
| page_fields | [PivotPageFields](/cells/es/python-net/aspose.cells.pivot/pivotpagefields) | Los elementos del campo de la página dinámica.|
| dest_cell_name | str | destCellName El nombre del nuevo informe de tabla dinámica.|
| table_name | str | el nombre del nuevo informe de tabla dinámica.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
Agrega un nuevo objeto de tabla dinámica a la colección con varios rangos de consolidación como fuente de datos.


###  Devoluciones

El nuevo índice de tabla dinámica agregado.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source_data | list | Los múltiples rangos de consolidación, como {"Hoja1!A1:C8","Hoja2!A1:B8"} |
| is_auto_page | bool | Si crea automáticamente un campo de una sola página.<br/> Si es verdadero, se ignorará el siguiente parámetro pageFields|
| page_fields | [PivotPageFields](/cells/es/python-net/aspose.cells.pivot/pivotpagefields) | Los elementos del campo de la página dinámica.|
| row | int | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| column | int | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica.|
| table_name | str | El nombre del nuevo informe de tabla dinámica.|



###  Ver también
* módulo [aspose.cells.pivot](../../)
* clase [PivotTableCollection](/cells/es/python-net/aspose.cells.pivot/pivottablecollection)
