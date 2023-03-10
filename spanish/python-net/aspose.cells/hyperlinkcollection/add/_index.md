---
title: add método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---
##  add(cell_name, total_rows, total_columns, address) {#str-int-int-str}
Agrega un hipervínculo a una celda específica o a un rango de celdas.


###  Devoluciones

[Hyperlink](/cells/es/python-net/aspose.cells/hyperlink) índice de objetos.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| cell_name | str | Cell nombre.|
| total_rows | int | Número de filas en este rango de hipervínculo.|
| total_columns | int | Número de columnas de este rango de hipervínculo.|
| address | str | Dirección del hipervínculo.|


##  add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}
Agrega un hipervínculo a una celda específica o a un rango de celdas.


###  Devoluciones

[Hyperlink](/cells/es/python-net/aspose.cells/hyperlink) índice de objetos.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| first_row | int | Primera fila del rango del hipervínculo.|
| first_column | int | Primera columna del rango del hipervínculo.|
| total_rows | int | Número de filas en este rango de hipervínculo.|
| total_columns | int | Número de columnas de este rango de hipervínculo.|
| address | str | Dirección del hipervínculo.|

###  Ejemplo

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


##  add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}
Agrega un hipervínculo a una celda específica o a un rango de celdas.


###  Devoluciones

[Hyperlink](/cells/es/python-net/aspose.cells/hyperlink) índice de objetos.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| start_cell_name | str | La celda superior izquierda del rango.|
| end_cell_name | str | La celda inferior derecha del rango.|
| address | str | Dirección del hipervínculo.|
| text_to_display | str | El texto que se mostrará para el hipervínculo especificado.|
| screen_tip | str |El texto de la información en pantalla para el hipervínculo especificado.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Hyperlink](/cells/es/python-net/aspose.cells/hyperlink)
* clase [HyperlinkCollection](/cells/es/python-net/aspose.cells/hyperlinkcollection)
