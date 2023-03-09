---
title: CustomDocumentPropertyCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  CustomDocumentPropertyCollection sınıfı
Özel belge özelliklerinden oluşan bir koleksiyon.



**Miras:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/tr/python-net/aspose.cells.properties/documentpropertycollection)



CustomDocumentPropertyCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [capacity](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [index_of(name)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Ada göre bir özelliğin dizinini alır.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [add(name, value)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | için yeni bir özel belge özelliği oluşturur.**PropertyType.String** veri tipi.|
| [add(name, value)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | için yeni bir özel belge özelliği oluşturur.**PropertyType.Number** veri tipi.|
| [add(name, value)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | için yeni bir özel belge özelliği oluşturur.**PropertyType.DateTime** veri tipi.|
| [add(name, value)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | için yeni bir özel belge özelliği oluşturur.**PropertyType.Boolean** veri tipi.|
| [add(name, value)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | için yeni bir özel belge özelliği oluşturur.**PropertyType.Floot** veri tipi.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|
| [add_link_to_content(name, source)](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | İçeriğe bağlanan yeni bir özel belge özelliği oluşturur.|
| [update_linked_property_value()](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) |İçeriğe bağlanan özel belge özellik değerini güncelleyin.|
| [update_linked_range()](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Özel belge özelliği değerini bağlantılı aralığa güncelleyin.|



###  Notlar

Her [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty) nesnesi, bir kapsayıcı belgenin özel bir özelliğini temsil eder.

###  örnekler

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Ayrıca bakınız
* modül [aspose.cells.properties](..)
* sınıf [CustomDocumentPropertyCollection](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection)
* sınıf [DocumentProperty](/cells/tr/python-net/aspose.cells.properties/documentproperty)
* sınıf [DocumentPropertyCollection](/cells/tr/python-net/aspose.cells.properties/documentpropertycollection)
