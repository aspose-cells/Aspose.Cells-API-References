---
title: PictureCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 460
url: /tr/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection sınıfı
[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne koleksiyonunu kapsüller.



PictureCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.drawing/picturecollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) | Koleksiyona bir resim ekler.|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) | Koleksiyona bir resim ekler.|
| [add(upper_left_row, upper_left_column, stream)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) | Koleksiyona bir resim ekler.|
| [add(upper_left_row, upper_left_column, file_name)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) | Koleksiyona bir resim ekler.|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) | Koleksiyona bir resim ekler.|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) | Koleksiyona bir resim ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
