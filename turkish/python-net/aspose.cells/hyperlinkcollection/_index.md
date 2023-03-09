---
title: HyperlinkCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 800
url: /tr/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
##  HyperlinkCollection sınıfı
[Hyperlink](/cells/tr/python-net/aspose.cells/hyperlink) nesne koleksiyonunu kapsüller.



HyperlinkCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells/hyperlinkcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) | Belirli bir hücreye veya bir hücre aralığına köprü ekler.|
| [add(cell_name, total_rows, total_columns, address)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) | Belirli bir hücreye veya bir hücre aralığına köprü ekler.|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) | Belirli bir hücreye veya bir hücre aralığına köprü ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  örnekler

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Hyperlink](/cells/tr/python-net/aspose.cells/hyperlink)
