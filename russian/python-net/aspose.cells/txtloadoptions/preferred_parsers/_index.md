---
title: preferred_parsers недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 300
url: /ru/python-net/aspose.cells/txtloadoptions/preferred_parsers/
is_root: false
---
##  preferred_parsers недвижимость

Получает и задает анализаторы предпочтительных значений для загрузки текстового файла.

###  Примечания

parsers[0] — парсер, который будет использоваться для первого столбца в текстовом файле шаблона,
parsers[1] — парсер, который будет использоваться для второго столбца и т. д.
Последний (parsers[parsers.length-1]) будет использоваться для всех остальных столбцов, начиная с parsers.length-1.
Если один элемент имеет значение null, соответствующий столбец будет проанализирован синтаксическим анализатором по умолчанию Aspose.Cells.
###  Определение:
```python
@property
def preferred_parsers(self):
    ...
@preferred_parsers.setter
def preferred_parsers(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [TxtLoadOptions](/cells/ru/python-net/aspose.cells/txtloadoptions)
