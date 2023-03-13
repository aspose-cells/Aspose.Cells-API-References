---
title: check_excel_restriction недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 80
url: /ru/python-net/aspose.cells/odsloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction недвижимость

Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками.
Например, Excel не позволяет вводить строковое значение длиннее 32 КБ.
Когда вы вводите значение длиннее 32 КБ, например, Cell.PutValue(строка), если это свойство истинно, вы получите исключение.
Если это свойство имеет значение false, мы примем значение вашей входной строки в качестве значения ячейки, чтобы позже
вы можете вывести полное строковое значение для файлов других форматов, таких как CSV.
Однако, если вы установили такое значение, которое недопустимо для формата файла Excel,
вы не должны сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel.
###  Определение:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [OdsLoadOptions](/cells/ru/python-net/aspose.cells/odsloadoptions)
