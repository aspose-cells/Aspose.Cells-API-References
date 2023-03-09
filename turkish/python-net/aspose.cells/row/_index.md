---
title: Row sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1300
url: /tr/python-net/aspose.cells/row/
is_root: false
---
##  Row sınıfı
Çalışma sayfasındaki tek bir satırı temsil eder.



Row türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_blank](/cells/tr/python-net/aspose.cells/row/is_blank) | Satırın herhangi bir veri içerip içermediğini gösterir|
| [is_collapsed](/cells/tr/python-net/aspose.cells/row/is_collapsed) | satırın daraltılmış olup olmadığı|
| [height](/cells/tr/python-net/aspose.cells/row/height) | Satır yüksekliğini Puan birimleri cinsinden alır ve ayarlar.|
| [is_hidden](/cells/tr/python-net/aspose.cells/row/is_hidden) | Satırın gizli olup olmadığını gösterir.|
| [index](/cells/tr/python-net/aspose.cells/row/index) | Bu satırın indeksini alır.|
| [group_level](/cells/tr/python-net/aspose.cells/row/group_level) | Satırın grup düzeyini alır.|
| [is_height_matched](/cells/tr/python-net/aspose.cells/row/is_height_matched) |Satır yüksekliği ile varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir.|
| [style](/cells/tr/python-net/aspose.cells/row/style) | Bu satırın stilini temsil eder.|
| [has_custom_style](/cells/tr/python-net/aspose.cells/row/has_custom_style) | Bu satırın özel stil ayarları olup olmadığını gösterir (çalışma kitabından devralınan varsayılandan farklı).|
| [first_cell](/cells/tr/python-net/aspose.cells/row/first_cell) | Satırdaki ilk hücre nesnesini alır.|
| [first_data_cell](/cells/tr/python-net/aspose.cells/row/first_data_cell) | Satırdaki ilk boş olmayan hücreyi alır.|
| [last_cell](/cells/tr/python-net/aspose.cells/row/last_cell) | Satırdaki son hücre nesnesini alır.|
| [last_data_cell](/cells/tr/python-net/aspose.cells/row/last_data_cell) | Satırdaki boş olmayan son hücreyi alır.|



Hücreyi alır.
###  İndeksleyici
| İsim| Tanım|
| :- | :- |
| [index] | sütun dizini|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_cell_by_index(index)](/cells/tr/python-net/aspose.cells/row/get_cell_by_index/#int) | Listedeki belirli dizine göre hücreyi alın.|
| [get_cell_or_null(column)](/cells/tr/python-net/aspose.cells/row/get_cell_or_null/#int) | Belirli dizindeki hücreyi veya boş değeri alır.|
| [get_style()](/cells/tr/python-net/aspose.cells/row/get_style/#) | Bu satırın stilini alır.|
| [set_style(style)](/cells/tr/python-net/aspose.cells/row/set_style/#Style) | Bu satırın stilini ayarlar.|
| [copy_settings(source, check_style)](/cells/tr/python-net/aspose.cells/row/copy_settings/#Row-bool) | Stil, yükseklik, görünürlük, vb. gibi satır ayarlarını kopyalayın.|
| [apply_style(style, flag)](/cells/tr/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Biçimleri tüm satıra uygular.|
| [equals(row)](/cells/tr/python-net/aspose.cells/row/equals/#Row) | Bu nesnenin başka bir satır nesnesiyle aynı satıra atıfta bulunup bulunmadığını kontrol eder.|



###  örnekler

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
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
