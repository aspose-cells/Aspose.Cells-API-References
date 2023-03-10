---
title: WorksheetCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1630
url: /tr/python-net/aspose.cells/worksheetcollection/
is_root: false
---
##  WorksheetCollection sınıfı
[Worksheet](/cells/tr/python-net/aspose.cells/worksheet) nesne koleksiyonunu kapsüller.



WorksheetCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [web_extension_task_panes](/cells/tr/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Görev bölmelerinin listesini alır.|
| [web_extensions](/cells/tr/python-net/aspose.cells/worksheetcollection/web_extensions) | Görev bölmelerinin listesini alır.|
| [threaded_comment_authors](/cells/tr/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Zincirleme yorum yazarlarının listesini alır.|
| [is_refresh_all_connections](/cells/tr/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Dosyayı MS Excel'de açarken tüm bağlantıların yenilenip yenilenmediğini gösterir.|
| [names](/cells/tr/python-net/aspose.cells/worksheetcollection/names) | Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır.|
| [active_sheet_name](/cells/tr/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Elektronik tablo açıldığında etkin çalışma sayfasının adını temsil eder.|
| [active_sheet_index](/cells/tr/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Elektronik tablo açıldığında etkin çalışma sayfasının dizinini temsil eder.|
| [dxfs](/cells/tr/python-net/aspose.cells/worksheetcollection/dxfs) | Ana diferansiyel biçimlendirme kayıtlarını alır.|
| [xml_maps](/cells/tr/python-net/aspose.cells/worksheetcollection/xml_maps) | Çalışma kitabındaki XML haritalarını alır ve ayarlar.|
| [built_in_document_properties](/cells/tr/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Elektronik tablonun tüm yerleşik belge özelliklerini temsil eden bir [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) koleksiyonunu döndürür.|
| [custom_document_properties](/cells/tr/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Elektronik tablonun tüm özel belge özelliklerini temsil eden bir [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) koleksiyonunu döndürür.|
| [ole_size](/cells/tr/python-net/aspose.cells/worksheetcollection/ole_size) | Çalışma Kitabı dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar.|
| [external_links](/cells/tr/python-net/aspose.cells/worksheetcollection/external_links) | Bir çalışma kitabındaki dış bağlantıları temsil eder.|
| [table_styles](/cells/tr/python-net/aspose.cells/worksheetcollection/table_styles) | [WorksheetCollection.table_styles](/cells/tr/python-net/aspose.cells/worksheetcollection#table_styles) nesnesini alır.|
| [revision_logs](/cells/tr/python-net/aspose.cells/worksheetcollection/revision_logs) |Revizyon günlüklerini temsil eder.|
| [capacity](/cells/tr/python-net/aspose.cells/worksheetcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get(index)](/cells/tr/python-net/aspose.cells/worksheetcollection/get/#int) |API for Python .Net yoluyla ekleyin, çünkü bu[int dizini] desteklenmiyor|
| [get(sheet_name)](/cells/tr/python-net/aspose.cells/worksheetcollection/get/#str) | API for Python .Net yoluyla ekleyin, çünkü bu [dize sayfasıAdı] desteklenmiyor|
| [add(type)](/cells/tr/python-net/aspose.cells/worksheetcollection/add/#SheetType) | Koleksiyona bir çalışma sayfası ekler.|
| [add()](/cells/tr/python-net/aspose.cells/worksheetcollection/add/#) | Koleksiyona bir çalışma sayfası ekler.|
| [add(sheet_name)](/cells/tr/python-net/aspose.cells/worksheetcollection/add/#str) | Koleksiyona bir çalışma sayfası ekler.|
| [register_add_in_function(add_in_file, function_name, lib)](/cells/tr/python-net/aspose.cells/worksheetcollection/register_add_in_function/#str-str-bool) | Çalışma kitabına eklenti işlevi ekler|
| [register_add_in_function(id, function_name)](/cells/tr/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-str) | Çalışma kitabına eklenti işlevi ekler|
| [add_copy(sheet_name)](/cells/tr/python-net/aspose.cells/worksheetcollection/add_copy/#str) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.|
| [add_copy(sheet_index)](/cells/tr/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.|
| [get_range_by_name(range_name)](/cells/tr/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str) | Önceden tanımlanmış ada göre Range nesnesini alır.|
| [get_range_by_name(range_name, current_sheet_index, include_table)](/cells/tr/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str-int-bool) | Önceden tanımlanmış ad veya tablo adına göre [Range](/cells/tr/python-net/aspose.cells/range)'i alır|
| [copy_to(array)](/cells/tr/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [create_range(address, sheet_index)](/cells/tr/python-net/aspose.cells/worksheetcollection/create_range/#str-int) | Aralığın adresinden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi oluşturur.|
| [create_union_range(address, sheet_index)](/cells/tr/python-net/aspose.cells/worksheetcollection/create_union_range/#str-int) | Aralığın adresinden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi oluşturur.|
| [get_sheet_by_code_name(code_name)](/cells/tr/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#str) | Çalışma sayfasını kod adına göre alır.|
| [sort_names()](/cells/tr/python-net/aspose.cells/worksheetcollection/sort_names/#) | Tanımlanan adları sıralar.|
| [swap_sheet(sheet_index1, sheet_index2)](/cells/tr/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | İki sayfayı değiştirir.|
| [remove_at(name)](/cells/tr/python-net/aspose.cells/worksheetcollection/remove_at/#str) | Belirli bir addaki öğeyi kaldırır.|
| [get_named_ranges()](/cells/tr/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Elektronik tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır.|
| [get_named_ranges_and_tables()](/cells/tr/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Elektronik tablodaki tüm önceden tanımlanmış adlandırılmış aralıkları alır.|
| [set_ole_size(start_row, end_row, start_column, end_column)](/cells/tr/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Çalışma Kitabı dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar.|
| [clear_pivottables()](/cells/tr/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Pivot tabloları e-tablodan temizler.|
| [refresh_pivot_tables()](/cells/tr/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) | WorksheetCollection içindeki tüm PivotTable'ları yeniler.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells/worksheetcollection/binary_search/#Worksheet) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook

workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
# Change the name of a worksheet
sheets[0].name = "First Sheet"
# Set the active sheet to the second worksheet
sheets.active_sheet_index = 1

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)
* sınıf [Worksheet](/cells/tr/python-net/aspose.cells/worksheet)
