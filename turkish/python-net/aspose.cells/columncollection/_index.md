---
title: ColumnCollection sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 270
url: /tr/python-net/aspose.cells/columncollection/
is_root: false
---
##  ColumnCollection sınıf
Bir çalışma sayfasındaki tek tek sütunları(ayarları) temsil eden [Column](/cells/tr/python-net/aspose.cells/column) nesnelerinin toplanması.
Column nesnesi yalnızca sütun genişliği, stiller, .vb. gibi ayarları temsil eder. tüm sütun için,
karşılık gelen sütunda boş olmayan hücrelerin (verilerin) olup olmamasıyla hiçbir ilgisi yoktur.
Ve bu koleksiyonun "Count" değeri yalnızca bu koleksiyonda başlatılmış olan Count Column nesnelerini temsil eder.
çalışma sayfasında boş olmayan hücrelerin (verilerin) olup olmamasıyla hiçbir ilgisi yoktur.



ColumnCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells/columncollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [copy_to(array)](/cells/tr/python-net/aspose.cells/columncollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells/columncollection/copy_to/#int-list-int-int) | Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells/columncollection/index_of/#Column-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells/columncollection/index_of/#Column-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells/columncollection/last_index_of/#Column) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells/columncollection/last_index_of/#Column-int) |Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells/columncollection/last_index_of/#Column-int-int) | Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [get_by_index(index)](/cells/tr/python-net/aspose.cells/columncollection/get_by_index/#int) | Sütun nesnesini dizine göre alır.|
| [get_column_by_index(index)](/cells/tr/python-net/aspose.cells/columncollection/get_column_by_index/#int) | Listedeki konuma göre [Column](/cells/tr/python-net/aspose.cells/column) nesnesini alır.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells/columncollection/binary_search/#Column) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Add new Style to Workbook
style = workbook.create_style()
# Setting the background color to Blue
style.foreground_color = Color.blue
# setting Background Pattern
style.pattern = BackgroundType.SOLID
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Change the default width of first ten columns
for i in range(10):
    worksheet.cells.columns[i].width = 20
# Get the Column with non default formatting
columns = worksheet.cells.columns
for column in columns:
    # Apply Style to first ten Columns
    column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Column](/cells/tr/python-net/aspose.cells/column)
