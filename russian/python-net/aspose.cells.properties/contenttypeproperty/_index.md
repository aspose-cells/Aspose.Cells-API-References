---
title: ContentTypeProperty класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.properties/contenttypeproperty/
is_root: false
---
##  ContentTypeProperty класс
Представляет информацию об идентификаторе.



Тип ContentTypeProperty предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [name](/cells/ru/python-net/aspose.cells.properties/contenttypeproperty/name) | Возвращает или задает имя объекта.|
| [value](/cells/ru/python-net/aspose.cells.properties/contenttypeproperty/value) | Возвращает или задает значение свойства типа контента.|
| [type](/cells/ru/python-net/aspose.cells.properties/contenttypeproperty/type) | Получает и задает тип свойства.|
| [is_nillable](/cells/ru/python-net/aspose.cells.properties/contenttypeproperty/is_nillable) | Указывает, может ли значение быть пустым.|



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
