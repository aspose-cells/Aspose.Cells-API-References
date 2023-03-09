---
title: start_access_cache метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 380
url: /ru/python-net/aspose.cells/workbook/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Запускает сеанс, который использует кэши для доступа к данным.



```python
def start_access_cache(self, opts):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/ru/python-net/aspose.cells/accesscacheoptions) | варианты доступа к данным|
###  Примечания

Если кеш указанного доступа к данным требует, чтобы некоторые модели данных на листе были доступны только для чтения,
тогда соответствующие модели данных на каждом листе в этой книге будут восприниматься как «только для чтения».
и пользователь не должен изменять ни один из них.


После завершения доступа к данным, [Workbook.close_access_cache(opts)](/cells/ru/python-net/aspose.cells/workbook/close_access_cache) должен
вызываться с теми же параметрами, чтобы очистить все кеши и восстановить нормальный режим доступа.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
