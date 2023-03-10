---
title: ChartCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection sınıfı
[Chart](/cells/tr/python-net/aspose.cells.charts/chart) nesne koleksiyonunu kapsüller.



ChartCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.charts/chartcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/tr/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) | Koleksiyona bir grafik ekler.|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/tr/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) | Koleksiyona bir grafik ekler.|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/tr/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) | Önceden ayarlanmış şablona sahip bir grafik ekler.|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/tr/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) | Koleksiyona bir grafik ekler.|
| [get(index)](/cells/tr/python-net/aspose.cells.charts/chartcollection/get/#int) |API for Python .Net yoluyla ekleyin, çünkü bu[int dizini] desteklenmiyor|
| [get(name)](/cells/tr/python-net/aspose.cells.charts/chartcollection/get/#str) | API for Python .Net yoluyla ekleyin, çünkü bu[dize Tablosu] desteklenmiyor|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [add_floating_chart(type, left, top, width, height)](/cells/tr/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) | Koleksiyona bir grafik ekler.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
* sınıf [Chart](/cells/tr/python-net/aspose.cells.charts/chart)
