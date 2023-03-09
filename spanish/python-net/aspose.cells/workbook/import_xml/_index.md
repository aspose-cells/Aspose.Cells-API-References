---
title: import_xml método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 220
url: /es/python-net/aspose.cells/workbook/import_xml/
is_root: false
---
##  import_xml(url, sheet_name, row, col) {#str-str-int-int}
Importa/actualiza un archivo de datos XML en el libro de trabajo.



```python
def import_xml(self, url, sheet_name, row, col):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| url | str | la url/ruta del archivo xml.|
| sheet_name | str | el nombre de la hoja de destino.|
| row | int | la fila de destino|
| col | int | la columna de destino|

###  Ejemplos

El siguiente código importa datos xml en la hoja de trabajo 'Hoja 1' en Cell A1.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
wb.import_xml("xml.xml", "Sheet1", 0, 0)
wb.save("output.xlsx")

```


##  import_xml(stream, sheet_name, row, col) {#io.RawIOBase-str-int-int}
Importa/actualiza un archivo de datos XML en el libro de trabajo.



```python
def import_xml(self, stream, sheet_name, row, col):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| stream | io.RawIOBase | la secuencia del archivo xml.|
| sheet_name | str | el nombre de la hoja de destino.|
| row | int | la fila de destino.|
| col | int | la columna de destino.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
