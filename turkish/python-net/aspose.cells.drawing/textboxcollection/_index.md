---
title: TextBoxCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 690
url: /tr/python-net/aspose.cells.drawing/textboxcollection/
is_root: false
---
##  TextBoxCollection sınıfı
[TextBox](/cells/tr/python-net/aspose.cells.drawing/textbox) nesne koleksiyonunu kapsüller.



TextBoxCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [copy_to(array)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/index_of/#TextBox-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#TextBox-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [add(upper_left_row, upper_left_column, height, width)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/add/#int-int-int-int) |Koleksiyona bir metin kutusu ekler.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.drawing/textboxcollection/binary_search/#TextBox) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get collection object
textBoxCollection = workbook.worksheets[0].text_boxes
# add a textbox
textBoxCollection.add(1, 1, 50, 100)
for tbox in textBoxCollection:
    pass

```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
* sınıf [TextBox](/cells/tr/python-net/aspose.cells.drawing/textbox)
