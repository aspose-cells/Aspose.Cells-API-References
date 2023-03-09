---
title: Column sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 260
url: /tr/python-net/aspose.cells/column/
is_root: false
---
##  Column sınıf
Çalışma sayfasındaki tek bir sütunu temsil eder.



Column türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [index](/cells/tr/python-net/aspose.cells/column/index) | Bu sütunun indeksini alır.|
| [width](/cells/tr/python-net/aspose.cells/column/width) | Karakter birimi cinsinden sütun genişliğini alır ve ayarlar.|
| [group_level](/cells/tr/python-net/aspose.cells/column/group_level) | Sütunun grup düzeyini alır.|
| [is_hidden](/cells/tr/python-net/aspose.cells/column/is_hidden) | Sütunun gizli olup olmadığını gösterir.|
| [has_custom_style](/cells/tr/python-net/aspose.cells/column/has_custom_style) | Bu sütunun özel stil ayarları olup olmadığını gösterir (çalışma kitabından devralınan varsayılandan farklı).|
| [style](/cells/tr/python-net/aspose.cells/column/style) | Bu sütunun stilini alır.|
| [is_collapsed](/cells/tr/python-net/aspose.cells/column/is_collapsed) | sütunun daraltılmış olup olmadığı|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [apply_style(style, flag)](/cells/tr/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Tüm sütun için biçimleri uygular.|
| [get_style()](/cells/tr/python-net/aspose.cells/column/get_style/#) | Bu sütunun stilini alır.|
| [set_style(style)](/cells/tr/python-net/aspose.cells/column/set_style/#Style) | Bu sütunun stilini ayarlar.|



###  Örnek

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first Column
column = worksheet.cells.columns[0]
# Apply Style to first Column
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
