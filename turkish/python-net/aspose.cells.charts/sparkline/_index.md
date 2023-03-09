---
title: Sparkline sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 260
url: /tr/python-net/aspose.cells.charts/sparkline/
is_root: false
---
##  Sparkline sınıf
Mini grafik, verilerin görsel bir temsilini sağlayan bir çalışma sayfası hücresindeki küçük bir grafiği veya grafiği temsil eder.



Sparkline türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [data_range](/cells/tr/python-net/aspose.cells.charts/sparkline/data_range) | Mini grafiğin veri aralığını temsil eder.|
| [row](/cells/tr/python-net/aspose.cells.charts/sparkline/row) | Mini grafiğin satır dizinini alır.|
| [column](/cells/tr/python-net/aspose.cells.charts/sparkline/column) | Mini grafiğin sütun dizinini alır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [to_image(file_name, options)](/cells/tr/python-net/aspose.cells.charts/sparkline/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) | Sparkline'ı görüntüye dönüştürür.|
| [to_image(stream, options)](/cells/tr/python-net/aspose.cells.charts/sparkline/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) | Sparkline'ı görüntüye dönüştürür.|



###  Örnek

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

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
