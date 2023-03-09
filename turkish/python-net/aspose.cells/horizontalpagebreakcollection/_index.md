---
title: HorizontalPageBreakCollection sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 760
url: /tr/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection sınıf
[HorizontalPageBreak](/cells/tr/python-net/aspose.cells/horizontalpagebreak) nesne koleksiyonunu kapsüller.



HorizontalPageBreakCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(row, start_column, end_column)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) | Koleksiyona yatay bir sayfa sonu ekler.|
| [add(row)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) | Koleksiyona yatay bir sayfa sonu ekler.|
| [add(row, column)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) | Koleksiyona yatay bir sayfa sonu ekler.|
| [add(cell_name)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) | Koleksiyona yatay bir sayfa sonu ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) | Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) |Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) | Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [HorizontalPageBreak](/cells/tr/python-net/aspose.cells/horizontalpagebreak)
