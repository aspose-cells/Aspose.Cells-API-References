---
title: ValidationCollection sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1550
url: /tr/python-net/aspose.cells/validationcollection/
is_root: false
---
##  ValidationCollection sınıf
Veri doğrulama koleksiyonunu temsil eder.



ValidationCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells/validationcollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add()](/cells/tr/python-net/aspose.cells/validationcollection/add/#) | Koleksiyona bir veri doğrulaması ekler.|
| [add(ca)](/cells/tr/python-net/aspose.cells/validationcollection/add/#CellArea) | Koleksiyona bir veri doğrulaması ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells/validationcollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) | Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells/validationcollection/index_of/#Validation-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells/validationcollection/last_index_of/#Validation) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) |Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) | Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [remove_a_cell(row, column)](/cells/tr/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) | Hücredeki tüm doğrulama ayarını kaldırır.|
| [remove_area(ca)](/cells/tr/python-net/aspose.cells/validationcollection/remove_area/#CellArea) | Aralıktaki tüm doğrulama ayarını kaldırır.|
| [get_validation_in_cell(row, column)](/cells/tr/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) | Verilen hücreye uygulanan doğrulamayı alır.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells/validationcollection/binary_search/#Validation) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
