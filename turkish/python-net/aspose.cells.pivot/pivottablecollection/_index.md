---
title: PivotTableCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 110
url: /tr/python-net/aspose.cells.pivot/pivottablecollection/
is_root: false
---
##  PivotTableCollection sınıfı
Belirtilen çalışma sayfasındaki tüm PivotTable nesnelerinin koleksiyonunu temsil eder.



PivotTableCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(source_data, dest_cell_name, table_name)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.|
| [add(source_data, dest_cell_name, table_name, use_same_source)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str-bool) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.|
| [add(source_data, row, column, table_name)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.|
| [add(source_data, row, column, table_name, use_same_source)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str-bool) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.|
| [add(pivot_table, dest_cell_name, table_name)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-str-str) | Koleksiyona başka bir PivotTable'dan yeni bir PivotTable Nesnesi ekler.|
| [add(pivot_table, row, column, table_name)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-int-int-str) | Koleksiyona başka bir PivotTable'dan yeni bir PivotTable Nesnesi ekler.|
| [add(source_data, is_auto_page, page_fields, dest_cell_name, table_name)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-str-str) | Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler.|
| [add(source_data, is_auto_page, page_fields, row, column, table_name)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-int-int-str) | Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [remove_at(index, keep_data)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | PivotTable'ı belirtilen dizinde siler|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#PivotTable) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  örnekler

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

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
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.pivot](..)
