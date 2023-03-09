---
title: classe Sparkline
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 260
url: /it/python-net/aspose.cells.charts/sparkline/
is_root: false
---
##  classe Sparkline
Un grafico sparkline rappresenta un piccolo grafico o grafico in una cella del foglio di lavoro che fornisce una rappresentazione visiva dei dati.



Il tipo Sparkline espone i membri seguenti:

###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [data_range](/cells/it/python-net/aspose.cells.charts/sparkline/data_range) | Rappresenta l'intervallo di dati del grafico sparkline.|
| [row](/cells/it/python-net/aspose.cells.charts/sparkline/row) | Ottiene l'indice di riga del grafico sparkline.|
| [column](/cells/it/python-net/aspose.cells.charts/sparkline/column) | Ottiene l'indice di colonna del grafico sparkline.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [to_image(file_name, options)](/cells/it/python-net/aspose.cells.charts/sparkline/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) | Converte un grafico sparkline in un'immagine.|
| [to_image(stream, options)](/cells/it/python-net/aspose.cells.charts/sparkline/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) | Converte un grafico sparkline in un'immagine.|



###  Esempi

```python
from aspose.cells import CellArea, Workbook
from aspose.cells.charts import SparklineType
from aspose.cells.rendering import ImageOrPrintOptions

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, sheet.name + "!A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
idx = group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
line = group.sparkline_collection[idx]
print("Saprkline data range: "  + line.data_range + ", row: "  + str(line.row) + ", column: "  + str(line.column))
line.to_image("output.png", ImageOrPrintOptions())

```

###  Guarda anche
* modulo [aspose.cells.charts](..)
