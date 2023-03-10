---
title: VbaModuleCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.vba/vbamodulecollection/
is_root: false
---
##  VbaModuleCollection sınıfı
[VbaModule](/cells/tr/python-net/aspose.cells.vba/vbamodule) listesini temsil eder



VbaModuleCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(sheet)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/add/#Worksheet) |Bir çalışma sayfası için modül ekler.|
| [add(type, name)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/add/#VbaModuleType-str) | Modül ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [add_designer_storage(name, data)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/add_designer_storage/#str-bytes) |  |
| [get_designer_storage(name)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/get_designer_storage/#str) | Tasarımcının verilerini temsil eder.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.vba/vbamodulecollection/binary_search/#VbaModule) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
vbaProject.modules.add(VbaModuleType.CLASS, "test")
# Saving the Excel file
workbook.save("book1.xlsm")

```

###  Ayrıca bakınız
* modül [aspose.cells.vba](..)
* sınıf [VbaModule](/cells/tr/python-net/aspose.cells.vba/vbamodule)
