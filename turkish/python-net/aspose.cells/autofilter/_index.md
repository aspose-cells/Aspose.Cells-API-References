---
title: AutoFilter sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 70
url: /tr/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter sınıfı
Belirtilen çalışma sayfası için otomatik filtrelemeyi temsil eder.



AutoFilter türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [sorter](/cells/tr/python-net/aspose.cells/autofilter/sorter) | Veri sıralayıcıyı alır.|
| [range](/cells/tr/python-net/aspose.cells/autofilter/range) | Belirtilen Otomatik Filtrenin uygulandığı aralığı temsil eder.|
| [show_filter_button](/cells/tr/python-net/aspose.cells/autofilter/show_filter_button) | Bu sütun için Otomatik Filtre düğmesinin görünür olup olmadığını belirtir.|
| [filter_columns](/cells/tr/python-net/aspose.cells/autofilter/filter_columns) | Filtre sütunlarının koleksiyonunu alır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/tr/python-net/aspose.cells/autofilter/remove_filter/#int-str) |Bir filtre sütunu için bir filtreyi kaldırır.|
| [remove_filter(field_index)](/cells/tr/python-net/aspose.cells/autofilter/remove_filter/#int) | Belirli filtreyi kaldırın.|
| [custom(field_index, operator_type1, criteria1)](/cells/tr/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Bir listeyi özel ölçütlerle filtreler.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/tr/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Bir listeyi özel ölçütlerle filtreler.|
| [refresh()](/cells/tr/python-net/aspose.cells/autofilter/refresh/#) | Satırları gizlemek veya göstermek için otomatik filtreleri yenileyin.|
| [refresh(hide_rows)](/cells/tr/python-net/aspose.cells/autofilter/refresh/#bool) | Tüm gizli satırların dizinlerini alır.|
| [set_range(row, start_column, end_column)](/cells/tr/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Belirtilen Otomatik Filtrenin uygulanacağı aralığı ayarlar.|
| [get_cell_area()](/cells/tr/python-net/aspose.cells/autofilter/get_cell_area/#) | Belirtilen AutoFilter'ın uygulandığı [CellArea](/cells/tr/python-net/aspose.cells/cellarea)'i alır.|
| [add_filter(field_index, criteria)](/cells/tr/python-net/aspose.cells/autofilter/add_filter/#int-str) | Bir filtre sütunu için bir filtre ekler.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/tr/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Bir tarih filtresi ekler.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/tr/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Bir tarih filtresini kaldırır.|
| [filter(field_index, criteria)](/cells/tr/python-net/aspose.cells/autofilter/filter/#int-str) | Bir listeyi belirtilen kriterlere göre filtreler.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/tr/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Listedeki ilk 10 öğeyi filtrele|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/tr/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Dinamik bir filtre ekler.|
| [add_font_color_filter(field_index, color)](/cells/tr/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Bir yazı tipi renk filtresi ekler.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/tr/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Bir dolgu rengi filtresi ekler.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/tr/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Bir simge filtresi ekler.|
| [match_blanks(field_index)](/cells/tr/python-net/aspose.cells/autofilter/match_blanks/#int) | Listedeki tüm boş hücreleri eşleştirin.|
| [match_non_blanks(field_index)](/cells/tr/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Listedeki tüm boş olmayan hücreleri eşleştirin.|
| [show_all()](/cells/tr/python-net/aspose.cells/autofilter/show_all/#) | Tüm satırları göster.|



###  Örnek

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [CellArea](/cells/tr/python-net/aspose.cells/cellarea)
