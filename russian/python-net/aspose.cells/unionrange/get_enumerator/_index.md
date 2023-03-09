---
title: get_enumerator метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/unionrange/get_enumerator/
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


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [UnionRange](/cells/ru/python-net/aspose.cells/unionrange)
