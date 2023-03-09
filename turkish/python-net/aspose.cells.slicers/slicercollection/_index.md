---
title: SlicerCollection sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells.slicers/slicercollection/
is_root: false
---
##  SlicerCollection sınıf
Belirtilen çalışma sayfasındaki tüm Slicer nesnelerinin koleksiyonunu belirtir.



SlicerCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.slicers/slicercollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(pivot, dest_cell_name, base_field_name)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-str) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin|
| [add(pivot, row, column, base_field_name)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-str) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin|
| [add(pivot, row, column, base_field_index)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-int) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin|
| [add(pivot, dest_cell_name, base_field_index)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-int) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin|
| [add(pivot, row, column, base_field)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin|
| [add(pivot, dest_cell_name, base_field)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField) | Veri kaynağı olarak PivotTable'ı kullanarak yeni bir Dilimleyici ekleyin|
| [add(table, index, dest_cell_name)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-int-str) | Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin|
| [add(table, list_column, dest_cell_name)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str) | Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin|
| [add(table, list_column, row, column)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int) | Veri kaynağı olarak ListObjet kullanarak yeni bir Dilimleyici ekleyin|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/copy_to/#int-list-int-int) | Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/index_of/#Slicer-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int) |Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/last_index_of/#Slicer-int-int) | Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.slicers/slicercollection/binary_search/#Slicer) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
tableIndex = sheet.list_objects.add("A1", "C9", True)
table = sheet.list_objects[tableIndex]
# do your business
book.save("out.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.slicers](..)
