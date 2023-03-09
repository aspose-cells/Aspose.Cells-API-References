---
title: get_enumerator метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 90
url: /ru/python-net/aspose.cells/range/get_enumerator/
is_root: false
---
##  get_enumerator() {#}
Получает перечислитель для ячеек в этом диапазоне.


###  Возвращает

Перечислитель ячеек


```python
def get_enumerator(self):
    ...
```


###  Примечания

При обходе элементов возвращаемым Enumerator коллекция ячеек
не следует изменять (например, операции, которые вызовут создание новой строки Cell/Row или удаление существующей строки Cell/Row).
В противном случае счетчик не сможет правильно пройти все ячейки (некоторые элементы могут быть пройдены повторно или пропущены).
###  Пример

```python
from aspose.cells import Workbook

workbook = Workbook("template.xlsx")
cells = workbook.worksheets[0].cells
en = cells.create_range("B2:C3").get_enumerator()
for cell in en:
    print(cell.name + ": "  + str(cell.value))

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Range](/cells/ru/python-net/aspose.cells/range)
