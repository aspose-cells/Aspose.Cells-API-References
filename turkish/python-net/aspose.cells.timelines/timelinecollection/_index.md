---
title: TimelineCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.timelines/timelinecollection/
is_root: false
---
##  TimelineCollection sınıfı
Belirtilen çalışma sayfasındaki tüm Zaman Çizelgesi nesnelerinin toplanmasını belirtir.
MS Excel nedeniyle Excel 2003, Zaman Çizelgesi'ni desteklemez.



TimelineCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(pivot, row, column, base_field_name)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin|
| [add(pivot, dest_cell_name, base_field_name)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-str) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin|
| [add(pivot, row, column, base_field_index)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin|
| [add(pivot, dest_cell_name, base_field_index)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-int) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin|
| [add(pivot, row, column, base_field)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin|
| [add(pivot, dest_cell_name, base_field)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Zaman Çizelgesi ekleyin|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/index_of/#Timeline-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#Timeline-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.timelines/timelinecollection/binary_search/#Timeline) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
import datetime

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.timelines](..)
