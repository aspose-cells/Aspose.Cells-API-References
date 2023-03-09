---
title: ExternalLink класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 560
url: /ru/python-net/aspose.cells/externallink/
is_root: false
---
##  ExternalLink класс
Представляет внешнюю ссылку в книге.



Тип ExternalLink предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [type](/cells/ru/python-net/aspose.cells/externallink/type) | Получает тип внешней ссылки.|
| [original_data_source](/cells/ru/python-net/aspose.cells/externallink/original_data_source) | Представляет сохраненный источник данных внешней ссылки.|
| [data_source](/cells/ru/python-net/aspose.cells/externallink/data_source) | Представляет источник данных внешней ссылки.|
| [is_referred](/cells/ru/python-net/aspose.cells/externallink/is_referred) | Указывает, ссылаются ли на эту внешнюю ссылку другие.|
| [is_visible](/cells/ru/python-net/aspose.cells/externallink/is_visible) | Указывает, видна ли эта внешняя ссылка в MS Excel.|


###  Методы
| Метод| Описание|
| :- | :- |
| [add_external_name(text, refer_to)](/cells/ru/python-net/aspose.cells/externallink/add_external_name/#str-str) | Добавляет внешнее имя.|



###  Примеры

```python
from aspose.cells import Workbook

# Open a file with external links
workbook = Workbook("book1.xls")
# Get External Link
externalLink = workbook.worksheets.external_links[0]
# Change External Link's Data Source
externalLink.data_source = "d:\\link.xls"

```

###  Смотрите также
* модуль [aspose.cells](..)
