---
title: FindOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 630
url: /tr/python-net/aspose.cells/findoptions/
is_root: false
---
##  FindOptions sınıfı
Bul seçeneklerini temsil eder.



FindOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [FindOptions()](/cells/tr/python-net/aspose.cells/findoptions/__init__/#) | FindOptions'ın yeni bir örneğini oluşturur|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_case_sensitive](/cells/tr/python-net/aspose.cells/findoptions/is_case_sensitive) | Aranan dizenin büyük/küçük harfe duyarlı olup olmadığını gösterir.|
| [case_sensitive](/cells/tr/python-net/aspose.cells/findoptions/case_sensitive) | Aranan dizenin büyük/küçük harfe duyarlı olup olmadığını gösterir.|
| [look_at_type](/cells/tr/python-net/aspose.cells/findoptions/look_at_type) | Tipe bak.|
| [is_range_set](/cells/tr/python-net/aspose.cells/findoptions/is_range_set) | Aranan aralığın ayarlanıp ayarlanmadığını gösterir.|
| [search_next](/cells/tr/python-net/aspose.cells/findoptions/search_next) | Arama sırası Doğru: sonrakini ara Yanlış: öncekini ara|
| [search_backward](/cells/tr/python-net/aspose.cells/findoptions/search_backward) | Hücreler için geriye doğru arama olup olmadığı.|
| [seach_order_by_rows](/cells/tr/python-net/aspose.cells/findoptions/seach_order_by_rows) | Arama sırasının satırlara mı yoksa sütunlara göre mi olduğunu gösterir.|
| [look_in_type](/cells/tr/python-net/aspose.cells/findoptions/look_in_type) | Tipe bak.|
| [regex_key](/cells/tr/python-net/aspose.cells/findoptions/regex_key) | Aranan anahtarın normal ifade olup olmadığını gösterir.<br/>True ise, aranan anahtar normal ifade olarak alınır ve ayrıştırılır.|
| [value_type_sensitive](/cells/tr/python-net/aspose.cells/findoptions/value_type_sensitive) | Aranan hücre değeri türünün aranan anahtarla aynı olup olmayacağını belirtir.|
| [style](/cells/tr/python-net/aspose.cells/findoptions/style) | Aranacak format.|
| [convert_numeric_data](/cells/tr/python-net/aspose.cells/findoptions/convert_numeric_data) | Aranan dize değerinin sayısal verilere dönüştürülüp dönüştürülmediğini gösteren bir değer alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_range()](/cells/tr/python-net/aspose.cells/findoptions/get_range/#) | Aranan aralığı alır ve ayarlar.|
| [set_range(ca)](/cells/tr/python-net/aspose.cells/findoptions/set_range/#CellArea) | Aranan aralığı ayarlar.|



###  örnekler

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
