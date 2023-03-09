---
title: metodo export_xml
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 140
url: /it/python-net/aspose.cells/workbook/export_xml/
is_root: false
---
##  export_xml(map_name, path) {#str-str}
Esporta i dati XML collegati dalla mappa XML specificata.



```python
def export_xml(self, map_name, path):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| map_name | str | nome della mappa XML che deve essere esportata|
| path | str | il percorso di esportazione|

###  Esempi

Il codice seguente ha esportato i dati collegati dal primo XmlMap.

```python
from aspose.cells import Workbook

wb = Workbook("Book1.xlsx")
# Make sure that the source xlsx file contains a XmlMap.
xmlMap = wb.worksheets.xml_maps[0]
wb.export_xml(xmlMap.name, "output.xml")

```


##  export_xml(map_name, stream) {#str-io.RawIOBase}
Esporta dati XML.



```python
def export_xml(self, map_name, stream):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| map_name | str | nome della mappa XML che deve essere esportata|
| stream | io.RawIOBase | il flusso di esportazione|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Workbook](/cells/it/python-net/aspose.cells/workbook)
