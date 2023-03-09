---
title: RowCollection sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1310
url: /tr/python-net/aspose.cells/rowcollection/
is_root: false
---
##  RowCollection sınıf
Bir çalışma sayfasındaki tek tek satırları temsil eden [Row](/cells/tr/python-net/aspose.cells/row) nesnelerini toplar.



RowCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [count](/cells/tr/python-net/aspose.cells/rowcollection/count) | Bu koleksiyondaki satır sayısını alır.|



Verilen satır dizinine göre bir [Row](/cells/tr/python-net/aspose.cells/row) nesnesi alır. Daha önce mevcut değilse, verilen satır dizininin Row nesnesi başlatılacaktır.
###  İndeksleyici
| İsim| Tanım|
| :- | :- |
| [index] |  |


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_row_by_index(index)](/cells/tr/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Satır nesnesini listedeki konuma göre alır.|
| [clear()](/cells/tr/python-net/aspose.cells/rowcollection/clear/#) | Tüm satırları ve hücreleri temizleyin.|
| [remove_at(index)](/cells/tr/python-net/aspose.cells/rowcollection/remove_at/#int) | Belirtilen dizindeki satırı kaldır|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Row](/cells/tr/python-net/aspose.cells/row)
