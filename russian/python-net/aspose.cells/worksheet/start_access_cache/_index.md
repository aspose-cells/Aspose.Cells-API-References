---
title: start_access_cache метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 280
url: /ru/python-net/aspose.cells/worksheet/start_access_cache/
is_root: false
---
##  start_access_cache(opts) {#AccessCacheOptions}
Запускает сеанс, использующий кэши для доступа к данным на этом листе.



```python
def start_access_cache(self, opts):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| opts | [AccessCacheOptions](/cells/ru/python-net/aspose.cells/accesscacheoptions) | варианты доступа к данным|
###  Примечания

После завершения доступа к данным, [Worksheet.close_access_cache(opts)](/cells/ru/python-net/aspose.cells/worksheet/close_access_cache) должен
вызываться с теми же параметрами, чтобы очистить все кеши и восстановить нормальный режим доступа.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [Worksheet](/cells/ru/python-net/aspose.cells/worksheet)
