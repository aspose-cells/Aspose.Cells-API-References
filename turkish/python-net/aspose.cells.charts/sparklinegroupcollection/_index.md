---
title: SparklineGroupCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 290
url: /tr/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  SparklineGroupCollection sınıfı
[SparklineGroup](/cells/tr/python-net/aspose.cells.charts/sparklinegroup) nesne koleksiyonunu kapsüller.



SparklineGroupCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [copy_to(array)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [add(type, data_range, is_vertical, location_range)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) | Koleksiyona bir [SparklineGroup](/cells/tr/python-net/aspose.cells.charts/sparklinegroup) öğe ekler.|
| [clear_sparklines(cell_area)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) | Bir hücre alanı içindeki mini çizgileri temizler.|
| [clear_sparkline_groups(cell_area)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) | Bir hücre alanıyla örtüşen mini grafik gruplarını temizler.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  örnekler

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType

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
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)

```

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
* sınıf [SparklineGroup](/cells/tr/python-net/aspose.cells.charts/sparklinegroup)
