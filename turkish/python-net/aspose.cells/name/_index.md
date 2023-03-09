---
title: Name sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1070
url: /tr/python-net/aspose.cells/name/
is_root: false
---
##  Name sınıf
Bir hücre aralığı için tanımlanmış bir adı temsil eder.



Name türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [comment](/cells/tr/python-net/aspose.cells/name/comment) | Adın yorumunu alır ve ayarlar.<br/> Yalnızca Excel 2007 için geçerlidir.|
| [text](/cells/tr/python-net/aspose.cells/name/text) | Nesnenin ad metnini alır.|
| [full_text](/cells/tr/python-net/aspose.cells/name/full_text) | Kapsam ayarı ile nesnenin adını tam metnini alır.|
| [refers_to](/cells/tr/python-net/aspose.cells/name/refers_to) | Adın başvurmak üzere tanımlandığı formülü, eşittir işaretiyle başlayarak döndürür veya ayarlar.|
| [r1c1_refers_to](/cells/tr/python-net/aspose.cells/name/r1c1_refers_to) | [Name](/cells/tr/python-net/aspose.cells/name)'in bir R1C1 referansını alır veya ayarlar.|
| [is_referred](/cells/tr/python-net/aspose.cells/name/is_referred) | Bu adın diğer formüller tarafından başvuruda bulunup bulunmadığını gösterir.|
| [is_visible](/cells/tr/python-net/aspose.cells/name/is_visible) | Adın görünür olup olmadığını gösterir.|
| [sheet_index](/cells/tr/python-net/aspose.cells/name/sheet_index) | Bu adın Çalışma Kitabı veya Çalışma Sayfasına ait olduğunu gösterir.<br/> 0 = Genel ad, aksi takdirde dizinden sayfaya (tek tabanlı)|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/name/get_refers_to/#bool-bool) | Bu İsmin referansını alın.|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/tr/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) | Belirtilen hücreye göre bu Adın referansını alın.|
| [get_ranges()](/cells/tr/python-net/aspose.cells/name/get_ranges/#) | Bu adla anılan tüm aralıkları alır.|
| [get_ranges(recalculate)](/cells/tr/python-net/aspose.cells/name/get_ranges/#bool) | Bu adla anılan tüm aralıkları alır.|
| [get_range()](/cells/tr/python-net/aspose.cells/name/get_range/#) | Bu ad bir aralığa başvuruyorsa aralığı alır.|
| [get_range(recalculate)](/cells/tr/python-net/aspose.cells/name/get_range/#bool) | Bu ad bir aralığa başvuruyorsa aralığı alır|
| [get_range(sheet_index, row, column)](/cells/tr/python-net/aspose.cells/name/get_range/#int-int-int) | Bu ad bir aralığa başvuruyorsa aralığı alır.<br/> Bu ismin referansı mutlak değilse, aralık farklı hücreler için farklı olabilir.|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) | Bu Adın referansını ayarlayın.|
| [get_referred_areas(recalculate)](/cells/tr/python-net/aspose.cells/name/get_referred_areas/#bool) | Bu adla anılan tüm başvuruları alır.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Name](/cells/tr/python-net/aspose.cells/name)
