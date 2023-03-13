---
title: WorkbookMetadata класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells.metadata/workbookmetadata/
is_root: false
---
##  WorkbookMetadata класс
Представляет метаданные.



Тип WorkbookMetadata предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [WorkbookMetadata(file_name, options)](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/__init__/#str-MetadataOptions) | Создайте объект метаданных.|
| [WorkbookMetadata(stream, options)](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/__init__/#io.RawIOBase-MetadataOptions) | Создайте объект метаданных.|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [options](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/options) | Получает параметры метаданных.|
| [built_in_document_properties](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/built_in_document_properties) |Возвращает коллекцию [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty), которая представляет все встроенные свойства документа электронной таблицы.|
| [custom_document_properties](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/custom_document_properties) | Возвращает коллекцию [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty), которая представляет все настраиваемые свойства документа электронной таблицы.|


###  Методы
| Метод| Описание|
| :- | :- |
| [save(file_name)](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/save/#str) | Сохраните измененные метаданные в файл.|
| [save(stream)](/cells/ru/python-net/aspose.cells.metadata/workbookmetadata/save/#io.RawIOBase) | Сохраните измененные метаданные в поток.|



###  Пример

В следующем примере создается файл WorkbookMetadata.

```python
from aspose.cells.metadata import MetadataOptions, MetadataType, WorkbookMetadata

options = MetadataOptions(MetadataType.DOCUMENT_PROPERTIES)
meta = WorkbookMetadata("book1.xlsx", options)
meta.custom_document_properties.add("test", "test")
meta.save("book2.xlsx")

```

###  Смотрите также
* модуль [aspose.cells.metadata](..)
* класс [DocumentProperty](/cells/ru/python-net/aspose.cells.properties/documentproperty)
