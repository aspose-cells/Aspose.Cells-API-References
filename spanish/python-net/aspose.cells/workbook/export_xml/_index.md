---
title: export_xml método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 140
url: /es/python-net/aspose.cells/workbook/export_xml/
is_root: false
---
##  export_xml(map_name, path) {#str-str}
Exportar datos XML vinculados por el mapa XML especificado.



```python
def export_xml(self, map_name, path):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| map_name | str | nombre del mapa XML que necesita ser exportado|
| path | str | la ruta de exportación|

###  Ejemplo

El siguiente código exportó los datos vinculados por el primer XmlMap.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")

```


##  export_xml(map_name, stream) {#str-io.RawIOBase}
Exportar datos XML.



```python
def export_xml(self, map_name, stream):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| map_name | str | nombre del mapa XML que necesita ser exportado|
| stream | io.RawIOBase | el flujo de exportación|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Workbook](/cells/es/python-net/aspose.cells/workbook)
