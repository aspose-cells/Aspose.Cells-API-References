---
title: ListObject sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells.tables/listobject/
is_root: false
---
##  ListObject sınıf
Çalışma sayfasındaki bir liste nesnesini temsil eder.
 ListObject nesnesi, ListObjects koleksiyonunun bir üyesidir.
ListObjects koleksiyonu, bir çalışma sayfasındaki tüm liste nesnelerini içerir.



ListObject türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [start_row](/cells/tr/python-net/aspose.cells.tables/listobject/start_row) | Aralığın başlangıç satırını alır.|
| [start_column](/cells/tr/python-net/aspose.cells.tables/listobject/start_column) | Aralığın başlangıç sütununu alır.|
| [end_row](/cells/tr/python-net/aspose.cells.tables/listobject/end_row) | Aralığın son satırını alır.|
| [end_column](/cells/tr/python-net/aspose.cells.tables/listobject/end_column) | Aralığın bitiş sütununu alır.|
| [list_columns](/cells/tr/python-net/aspose.cells.tables/listobject/list_columns) | ListObject öğesinin ListColumns değerini alır.|
| [show_header_row](/cells/tr/python-net/aspose.cells.tables/listobject/show_header_row) | Bu ListObject başlık satırını gösterip göstermediğini alır ve ayarlar.|
| [show_totals](/cells/tr/python-net/aspose.cells.tables/listobject/show_totals) |Bu ListObject'in toplam satırı gösterip göstermediğini alır ve ayarlar.|
| [data_range](/cells/tr/python-net/aspose.cells.tables/listobject/data_range) | ListObject veri aralığını alır.|
| [query_table](/cells/tr/python-net/aspose.cells.tables/listobject/query_table) |Bağlantılı QueryTable'ı alır.|
| [data_source_type](/cells/tr/python-net/aspose.cells.tables/listobject/data_source_type) | Tablonun veri kaynağı türünü alır.|
| [auto_filter](/cells/tr/python-net/aspose.cells.tables/listobject/auto_filter) | Otomatik filtre alır.|
| [display_name](/cells/tr/python-net/aspose.cells.tables/listobject/display_name) | Görünen adı alır ve ayarlar.|
| [comment](/cells/tr/python-net/aspose.cells.tables/listobject/comment) | Tablonun yorumunu alır ve ayarlar.|
| [show_table_style_first_column](/cells/tr/python-net/aspose.cells.tables/listobject/show_table_style_first_column) | Tablodaki ilk sütuna stilin uygulanıp uygulanmayacağını belirtir.|
| [show_table_style_last_column](/cells/tr/python-net/aspose.cells.tables/listobject/show_table_style_last_column) | Tablodaki son sütuna stilin uygulanıp uygulanmayacağını belirtir.|
| [show_table_style_row_stripes](/cells/tr/python-net/aspose.cells.tables/listobject/show_table_style_row_stripes) | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir.|
| [show_table_style_column_stripes](/cells/tr/python-net/aspose.cells.tables/listobject/show_table_style_column_stripes) | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir.|
| [table_style_type](/cells/tr/python-net/aspose.cells.tables/listobject/table_style_type) | Alır ve yerleşik tablo stili.|
| [table_style_name](/cells/tr/python-net/aspose.cells.tables/listobject/table_style_name) | Tablo stili adını alır ve ayarlar.|
| [xml_map](/cells/tr/python-net/aspose.cells.tables/listobject/xml_map) | Bu liste için kullanılan bir [ListObject.xml_map](/cells/tr/python-net/aspose.cells.tables/listobject#xml_map) alır.|
| [alternative_text](/cells/tr/python-net/aspose.cells.tables/listobject/alternative_text) | Alternatif metni alır ve ayarlar.|
| [alternative_description](/cells/tr/python-net/aspose.cells.tables/listobject/alternative_description) | Alternatif açıklamayı alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [convert_to_range()](/cells/tr/python-net/aspose.cells.tables/listobject/convert_to_range/#) | Tabloyu aralığa dönüştürün.|
| [convert_to_range(options)](/cells/tr/python-net/aspose.cells.tables/listobject/convert_to_range/#TableToRangeOptions) | Tabloyu aralığa dönüştürün.|
| [resize(start_row, start_column, end_row, end_column, has_headers)](/cells/tr/python-net/aspose.cells.tables/listobject/resize/#int-int-int-int-bool) | Liste nesnesinin aralığını yeniden boyutlandırın.|
| [put_cell_value(row_offset, column_offset, value)](/cells/tr/python-net/aspose.cells.tables/listobject/put_cell_value/#int-int-any) | Değeri hücreye koyun.|
| [update_column_name()](/cells/tr/python-net/aspose.cells.tables/listobject/update_column_name/#) |Çalışma sayfasındaki tüm liste sütunlarının adını günceller.|
| [filter()](/cells/tr/python-net/aspose.cells.tables/listobject/filter/#) | Tabloyu filtreleyin.|
| [apply_style_to_range()](/cells/tr/python-net/aspose.cells.tables/listobject/apply_style_to_range/#) | Tablo stilini aralığa uygulayın.|



###  Örnek

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(5):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
table.list_columns[4].totals_calculation = TotalsCalculation.SUM
workbook.save(r"Book1.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.tables](..)
