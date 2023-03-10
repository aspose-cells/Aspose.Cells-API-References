---
title: ContentTypePropertyCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.properties/contenttypepropertycollection/
is_root: false
---
##  ContentTypePropertyCollection класс
Коллекция из [ContentTypeProperty](/cells/ru/python-net/aspose.cells.properties/contenttypeproperty) объектов, представляющих дополнительную информацию.



Тип ContentTypePropertyCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [capacity](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/capacity) | Получает или задает количество элементов, которые может содержать список массивов.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(name, value)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str) | Добавляет информацию о свойстве типа контента.|
| [add(name, value, type)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/add/#str-str-str) | Добавляет информацию о свойстве типа контента.|
| [copy_to(array)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#list) | Копирует весь список массивов в совместимый список одномерных массивов, начиная с начала целевого списка массивов.|
| [copy_to(index, array, array_index, count)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/copy_to/#int-list-int-int) |Копирует диапазон элементов из списка массивов в совместимый список одномерных массивов, начиная с указанного индекса целевого списка массивов.|
| [index_of(item, index)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который простирается от указанного индекса до последнего элемента.|
| [index_of(item, index, count)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/index_of/#ContentTypeProperty-int-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс первого вхождения в диапазоне элементов в списке массивов, который начинается с указанного индекса и содержит указанное количество элементов.|
| [last_index_of(item)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения во всем списке массивов.|
| [last_index_of(item, index)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int) | Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который простирается от первого элемента до указанного индекса.|
| [last_index_of(item, index, count)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/last_index_of/#ContentTypeProperty-int-int) |Выполняет поиск указанного объекта и возвращает отсчитываемый от нуля индекс последнего вхождения в диапазоне элементов в списке массивов, который содержит указанное количество элементов и заканчивается указанным индексом.|
| [binary_search(item)](/cells/ru/python-net/aspose.cells.properties/contenttypepropertycollection/binary_search/#ContentTypeProperty) | Ищет элемент во всем отсортированном списке массивов, используя компаратор по умолчанию, и возвращает отсчитываемый от нуля индекс элемента.|



###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Add a new property.
workbook.content_type_properties.add("Admin", "Aspose", "text")
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Смотрите также
* модуль [aspose.cells.properties](..)
* класс [ContentTypeProperty](/cells/ru/python-net/aspose.cells.properties/contenttypeproperty)
