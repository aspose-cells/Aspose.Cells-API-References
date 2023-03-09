---
title: ExternalLinkCollection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 570
url: /ru/python-net/aspose.cells/externallinkcollection/
is_root: false
---
##  ExternalLinkCollection класс
Представляет коллекцию внешних ссылок в книге.



Тип ExternalLinkCollection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [count](/cells/ru/python-net/aspose.cells/externallinkcollection/count) | Получает количество элементов, фактически содержащихся в коллекции.|



Получает элемент [ExternalLink](/cells/ru/python-net/aspose.cells/externallink) по указанному индексу.
###  Индексатор
| Имя| Описание|
| :- | :- |
| [index] | Отсчитываемый от нуля индекс элемента.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add(file_name, sheet_names)](/cells/ru/python-net/aspose.cells/externallinkcollection/add/#str-list) | Добавляет внешнюю ссылку.|
| [add(directory_type, file_name, sheet_names)](/cells/ru/python-net/aspose.cells/externallinkcollection/add/#DirectoryType-str-list) | Добавьте внешнюю ссылку.|
| [clear()](/cells/ru/python-net/aspose.cells/externallinkcollection/clear/#) | Удаляет все внешние ссылки.|
| [clear(update_references_as_local)](/cells/ru/python-net/aspose.cells/externallinkcollection/clear/#bool) | Удаляет все внешние ссылки.|
| [remove_at(index)](/cells/ru/python-net/aspose.cells/externallinkcollection/remove_at/#int) | Удаляет указанную внешнюю ссылку из книги.|
| [remove_at(index, update_references_as_local)](/cells/ru/python-net/aspose.cells/externallinkcollection/remove_at/#int-bool) | Удаляет указанную внешнюю ссылку из книги.|



###  Пример

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Change external link data source
workbook.worksheets.external_links[0].data_source = "d:\\link.xls"

```

###  Смотрите также
* модуль [aspose.cells](..)
* класс [ExternalLink](/cells/ru/python-net/aspose.cells/externallink)
