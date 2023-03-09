---
title: CustomDocumentPropertyCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.properties/customdocumentpropertycollection/
is_root: false
---
##  CustomDocumentPropertyCollection класс
Коллекция настраиваемых свойств документа.



**Наследование:** [CustomDocumentPropertyCollection](/cells/python-net/aspose.cells.properties/customdocumentpropertycollection) → 
[DocumentPropertyCollection](/cells/ru/python-net/aspose.cells.properties/documentpropertycollection)



Тип CustomDocumentPropertyCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [index_of(name)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#str) | Получает индекс свойства по имени.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/index_of/#DocumentProperty-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/copy_to/#int-list-int-int) | Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/last_index_of/#DocumentProperty-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [add(name, value)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-str) | Создает новое пользовательское свойство документа**Тип свойства.String** тип данных.|
| [add(name, value)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-int) | Создает новое пользовательское свойство документа**PropertyType.Number** тип данных.|
| [add(name, value)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-DateTime) | Создает новое пользовательское свойство документа**PropertyType.DateTime** тип данных.|
| [add(name, value)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-bool) | Создает новое пользовательское свойство документа**PropertyType.Boolean** тип данных.|
| [add(name, value)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/add/#str-float) | Создает новое пользовательское свойство документа**PropertyType.Float** тип данных.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/binary_search/#DocumentProperty) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|
| [add_link_to_content(name, source)](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/add_link_to_content/#str-str) | Создает новое пользовательское свойство документа, которое ссылается на содержимое.|
| [update_linked_property_value()](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_property_value/#) | Обновите значение пользовательского свойства документа, которое ссылается на содержимое.|
| [update_linked_range()](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection/update_linked_range/#) | Обновите значение пользовательского свойства документа до связанного диапазона.|



###  Примечания

Каждый объект [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty) представляет пользовательское свойство документа-контейнера.

###  Пример

```python
from aspose.cells import Workbook

# Instantiate a Workbook object
workbook = Workbook("book1.xls")
# Retrieve a list of all custom document properties of the Excel file
customProperties = workbook.worksheets.custom_document_properties

```

###  Смотрите также
* модуль [aspose.cells.properties](..)
* класс [CustomDocumentPropertyCollection](/cells/ru/python-net/aspose.cells.properties/customdocumentpropertycollection)
* класс [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty)
* класс [DocumentPropertyCollection](/cells/ru/python-net/aspose.cells.properties/documentpropertycollection)
