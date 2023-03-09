---
title: multi_thread_reading недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1200
url: /ru/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading недвижимость

Получает или задает, должна ли модель данных ячеек поддерживать многопоточное чтение.
Значение по умолчанию этого свойства — false.

###  Примечания

Если есть несколько потоков для одновременного чтения объектов Row/Cell в этой коллекции,
это свойство должно быть установлено как true, в противном случае может быть получен неожиданный результат.
Поддержка многопоточного чтения может снизить производительность доступа к объектам Row/Cell из этой коллекции.
Обратите внимание, что некоторые функции не поддерживают многопоточное чтение.
такие как значения форматирования (по [Cell.string_value](/cells/ru/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/ru/python-net/aspose.cells/cell#display_string_value) и т. д.).
Таким образом, даже если для этого свойства задано значение true, эти API-интерфейсы по-прежнему могут давать неожиданный результат для многопоточного чтения.
###  Определение:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Cells](/cells/ru/python-net/aspose.cells/cells)
