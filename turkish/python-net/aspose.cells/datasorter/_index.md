---
title: DataSorter sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 420
url: /tr/python-net/aspose.cells/datasorter/
is_root: false
---
##  DataSorter sınıfı
DataSorter için özet açıklama.



DataSorter türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [keys](/cells/tr/python-net/aspose.cells/datasorter/keys) | Veri sıralayıcının anahtar listesini alır.|
| [has_headers](/cells/tr/python-net/aspose.cells/datasorter/has_headers) | Aralığın başlıkları olup olmadığını temsil eder.|
| [key1](/cells/tr/python-net/aspose.cells/datasorter/key1) | İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0'dır, B 1'dir, ...).|
| [order1](/cells/tr/python-net/aspose.cells/datasorter/order1) | İlk anahtarın sıralama düzenini temsil eder.|
| [key2](/cells/tr/python-net/aspose.cells/datasorter/key2) | İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0'dır, B 1'dir, ...).|
| [order2](/cells/tr/python-net/aspose.cells/datasorter/order2) | İkinci anahtarın sıralama düzenini temsil eder.|
| [key3](/cells/tr/python-net/aspose.cells/datasorter/key3) | Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0'dır, B 1'dir, ...).|
| [order3](/cells/tr/python-net/aspose.cells/datasorter/order3) | Üçüncü anahtarın sıralama düzenini temsil eder.|
| [sort_left_to_right](/cells/tr/python-net/aspose.cells/datasorter/sort_left_to_right) | Doğru, sıralama yönünün soldan sağa olduğu anlamına gelir.<br/>Yanlış, sıralama yönünün yukarıdan aşağıya olduğu anlamına gelir.<br/> Varsayılan değer yanlıştır.|
| [case_sensitive](/cells/tr/python-net/aspose.cells/datasorter/case_sensitive) | Dizeyi karşılaştırırken büyük/küçük harfe duyarlı olup olmadığını alır ve ayarlar.|
| [sort_as_number](/cells/tr/python-net/aspose.cells/datasorter/sort_as_number) | Sayı gibi görünen herhangi bir şeyin sıralanıp sıralanmadığını gösterir.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add_key(key, order)](/cells/tr/python-net/aspose.cells/datasorter/add_key/#int-SortOrder) | Sıralanmış sütun dizini ve sıralama düzeni ekler.|
| [add_key(key, order, custom_list)](/cells/tr/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-str) | Özel sıralama listesiyle sıralanmış sütun dizini ve sıralama düzeni ekler.|
| [add_key(key, type, order, custom_list)](/cells/tr/python-net/aspose.cells/datasorter/add_key/#int-SortOnType-SortOrder-any) | Özel sıralama listesiyle sıralanmış sütun dizini ve sıralama düzeni ekler.|
| [add_key(key, order, custom_list)](/cells/tr/python-net/aspose.cells/datasorter/add_key/#int-SortOrder-list) | Özel sıralama listesiyle sıralanmış sütun dizini ve sıralama düzeni ekler.|
| [sort(cells, start_row, start_column, end_row, end_column)](/cells/tr/python-net/aspose.cells/datasorter/sort/#Cells-int-int-int-int) | Alanın verilerini sıralar.|
| [sort(cells, area)](/cells/tr/python-net/aspose.cells/datasorter/sort/#Cells-CellArea) | Alanın verilerini sıralayın.|
| [sort()](/cells/tr/python-net/aspose.cells/datasorter/sort/#) | Aralıktaki verileri sıralayın.|
| [clear()](/cells/tr/python-net/aspose.cells/datasorter/clear/#) | Tüm ayarları temizleyin.|



###  Örnek

```python
from aspose.cells import CellArea, SortOrder, Workbook

# Instantiate a new Workbook object.
workbook = Workbook("Book1.xls")
# Get the workbook datasorter object.
sorter = workbook.data_sorter
# Set the first order for datasorter object.
sorter.order1 = SortOrder.DESCENDING
# Define the first key.
sorter.key1 = 0
# Set the second order for datasorter object.
sorter.order2 = SortOrder.ASCENDING
# Define the second key.
sorter.key2 = 1
# Create a cells area (range).
ca = CellArea()
# Specify the start row index.
ca.start_row = 0
# Specify the start column index.
ca.start_column = 0
# Specify the last row index.
ca.end_row = 13
# Specify the last column index.
ca.end_column = 1
# Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets[0].cells, ca)
# Save the excel file.
workbook.save("outBook.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
