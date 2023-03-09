---
title: DataBar sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 400
url: /tr/python-net/aspose.cells/databar/
is_root: false
---
##  DataBar sınıf
 DataBar koşullu biçimlendirme kuralını açıklayın.
Bu koşullu biçimlendirme kuralı, derecelendirilmiş bir
hücre aralığındaki veri çubuğu.



DataBar türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [axis_color](/cells/tr/python-net/aspose.cells/databar/axis_color) | Veri çubukları olarak koşullu biçimlendirmeye sahip hücreler için eksen rengini alır.|
| [axis_position](/cells/tr/python-net/aspose.cells/databar/axis_position) | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının ekseninin konumunu alır veya ayarlar.|
| [bar_fill_type](/cells/tr/python-net/aspose.cells/databar/bar_fill_type) | Bir veri çubuğunun renkle nasıl doldurulacağını alır veya ayarlar.|
| [direction](/cells/tr/python-net/aspose.cells/databar/direction) | Veri çubuğunun görüntülenme yönünü alır veya ayarlar.|
| [bar_border](/cells/tr/python-net/aspose.cells/databar/bar_border) | Veri çubuğunun kenarlığını belirten bir nesne alır.|
| [negative_bar_format](/cells/tr/python-net/aspose.cells/databar/negative_bar_format) | Bir veri çubuğu koşullu biçimlendirme kuralıyla ilişkili NegativeBarFormat nesnesini alır.|
| [min_cfvo](/cells/tr/python-net/aspose.cells/databar/min_cfvo) | Bu DataBar'ın minimum değer nesnesini alın veya ayarlayın.<br/> FormatConditionValueType.Max türünde null veya CFValueObject ayarlanamıyor.|
| [max_cfvo](/cells/tr/python-net/aspose.cells/databar/max_cfvo) | Bu DataBar'ın maksimum değer nesnesini alın veya ayarlayın.<br/> FormatConditionValueType.Min türünde null veya CFValueObject ayarlanamıyor.|
| [color](/cells/tr/python-net/aspose.cells/databar/color) | Bu DataBar'ın Rengini alın veya ayarlayın.|
| [min_length](/cells/tr/python-net/aspose.cells/databar/min_length) | Veri çubuğunun minimum uzunluğunu temsil eder.|
| [max_length](/cells/tr/python-net/aspose.cells/databar/max_length) | Veri çubuğunun maksimum uzunluğunu temsil eder.|
| [show_value](/cells/tr/python-net/aspose.cells/databar/show_value) | Bu veri çubuğunun uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini gösteren bayrağı alın veya ayarlayın.<br/> Varsayılan değer doğrudur.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [to_image(cell, img_opts)](/cells/tr/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | Görüntü bayt dizisine hücredeki veri çubuğunu işleyin.|



###  Örnek

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
