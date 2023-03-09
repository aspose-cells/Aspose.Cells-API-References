---
title: check_font_compatibility недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 50
url: /ru/python-net/aspose.cells/xpssaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility недвижимость

Указывает, следует ли проверять совместимость шрифтов для каждого символа в тексте.

###  Примечания

Значение по умолчанию верно.
Отключение этого свойства может повысить производительность.
Но когда для его отображения нельзя использовать заданный по умолчанию или указанный шрифт текста/символа,
нечитаемые символы (например, блок) могут встречаться в сгенерированном PDF-файле.
В такой ситуации пользователь должен сохранить это свойство как true, чтобы
альтернативный шрифт можно найти и использовать для отображения текста вместо него;
###  Определение:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [XpsSaveOptions](/cells/ru/python-net/aspose.cells/xpssaveoptions)
