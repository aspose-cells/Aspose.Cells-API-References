---
title: IconSet sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 900
url: /tr/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet sınıfı
 IconSet koşullu biçimlendirme kuralını açıklayın.
Bu koşullu biçimlendirme kuralı, simgeleri hücrelere uygular
değerlerine göre.



IconSet türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [cf_icons](/cells/tr/python-net/aspose.cells/iconset/cf_icons) | Koleksiyondan [ConditionalFormattingIcon](/cells/tr/python-net/aspose.cells/conditionalformattingicon)'i edinin|
| [cfvos](/cells/tr/python-net/aspose.cells/iconset/cfvos) | CFValueObjects örneğini alın.|
| [type](/cells/tr/python-net/aspose.cells/iconset/type) | Görüntülenecek simge seti türünü alın veya ayarlayın.<br/>Türün ayarlanması, geçerli Cfvos sayısının olup olmadığını otomatik olarak kontrol edecektir.<br/> yeni tipe uygun. Uyulmadığı takdirde eski Cfvos temizlenecek ve<br/> varsayılan Cfvos eklenecektir.|
| [is_custom](/cells/tr/python-net/aspose.cells/iconset/is_custom) | Simge setinin özel olup olmadığını gösterir.<br/> Varsayılan değer yanlıştır.|
| [show_value](/cells/tr/python-net/aspose.cells/iconset/show_value) | Bu simge setinin uygulandığı hücrelerin değerlerinin gösterilip gösterilmeyeceğini gösteren bayrağı alın veya ayarlayın.<br/> Varsayılan değer doğrudur.|
| [reverse](/cells/tr/python-net/aspose.cells/iconset/reverse) | Bu simge setindeki simgelerin varsayılan sırasının tersine çevrilip çevrilmeyeceğini gösteren bayrağı alın veya ayarlayın.<br/> Varsayılan değer yanlıştır.|



###  Örnek

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

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
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]
# Get Icon Set
iconSet = cond.icon_set
# Set Icon Type
iconSet.type = IconSetType.ARROWS3
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
* sınıf [ConditionalFormattingIcon](/cells/tr/python-net/aspose.cells/conditionalformattingicon)
