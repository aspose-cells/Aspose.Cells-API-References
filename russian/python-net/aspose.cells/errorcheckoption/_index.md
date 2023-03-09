---
title: ErrorCheckOption класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 520
url: /ru/python-net/aspose.cells/errorcheckoption/
is_root: false
---
##  ErrorCheckOption класс
Параметр проверки ошибок применяется к определенным диапазонам.



Тип ErrorCheckOption предоставляет следующие члены:

###  Методы
| Метод| Описание|
| :- | :- |
| [is_error_check(error_check_type)](/cells/ru/python-net/aspose.cells/errorcheckoption/is_error_check/#ErrorCheckType) | Проверяет, будет ли проверяться данный тип ошибки.|
| [set_error_check(error_check_type, is_check)](/cells/ru/python-net/aspose.cells/errorcheckoption/set_error_check/#ErrorCheckType-bool) | Устанавливает, будет ли проверяться данный тип ошибки.|
| [get_count_of_range()](/cells/ru/python-net/aspose.cells/errorcheckoption/get_count_of_range/#) | Получает количество диапазонов, на которые повлиял этот параметр.|
| [add_range(ca)](/cells/ru/python-net/aspose.cells/errorcheckoption/add_range/#CellArea) | Добавляет один диапазон, на который влияет этот параметр.|
| [get_range(index)](/cells/ru/python-net/aspose.cells/errorcheckoption/get_range/#int) | Получает диапазон влияния этого параметра по заданному индексу.|
| [remove_range(index)](/cells/ru/python-net/aspose.cells/errorcheckoption/remove_range/#int) | Удаляет один диапазон по заданному индексу.|



###  Пример

```python
from aspose.cells import CellArea, ErrorCheckType, Workbook

workbook = Workbook()
opts = workbook.worksheets[0].error_check_options
optionIdx = opts.add()
opt = opts[optionIdx]
opt.set_error_check(ErrorCheckType.INCONSIST_FORMULA, False)
opt.set_error_check(ErrorCheckType.INCONSIST_RANGE, False)
opt.set_error_check(ErrorCheckType.TEXT_DATE, False)
opt.set_error_check(ErrorCheckType.TEXT_NUMBER, False)
opt.set_error_check(ErrorCheckType.VALIDATION, False)
opt.add_range(CellArea.create_cell_area("A1", "B10"))
workbook.save(r"Book1.xlsx")

```

###  Смотрите также
* модуль [aspose.cells](..)
