---
title: Top10 sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1480
url: /tr/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 sınıf
 Top10 koşullu biçimlendirme kuralını açıklayın.
Bu koşullu biçimlendirme kuralı,
değerler, belirtildiği gibi üst N veya alt N köşeli parantez içinde yer alır.



Top10 türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [Top10()](/cells/tr/python-net/aspose.cells/top10/__init__/#) | Top10'un yeni bir örneğini oluşturur|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_percent](/cells/tr/python-net/aspose.cells/top10/is_percent) | "Üst/alt n" kuralının "yüzde üst/alt n" kuralı olup olmadığını alın veya ayarlayın.<br/> Varsayılan değer yanlıştır.|
| [is_bottom](/cells/tr/python-net/aspose.cells/top10/is_bottom) | Bir "üst/alt n" kuralının bir "alt n" kuralı olup olmadığını alın veya ayarlayın.<br/> Varsayılan değer yanlıştır.|
| [rank](/cells/tr/python-net/aspose.cells/top10/rank) | "Üst/alt n" koşullu biçimlendirme kuralında "n" değerini alın veya ayarlayın.<br/>IsPercent true ise, değer 0 ile 100 arasında olmalıdır.<br/>Aksi takdirde 0 ile 1000 arasında olmalıdır.<br/> Varsayılan değer 10'dur.|



###  Örnek

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
