---
title: "Класс GridCacheForStream"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridJs.GridCacheForStream class. Этот класс содержит операции кеша для GridJs. Пользователь должен реализовать свою бизнес‑логику хранения, основываясь на нём"
type: docs
url: /ru/net/aspose.cells.gridjs/gridcacheforstream/
---
## GridCacheForStream class

Этот класс содержит операции кэширования для GridJs. Пользователь должен реализовать свою бизнес‑логику хранения на его основе..

```csharp
public abstract class GridCacheForStream
```

## Методы

| Имя | Описание |
| --- | --- |
| abstract [GetFileUrl](../../aspose.cells.gridjs/gridcacheforstream/getfileurl/)(string) | Реализует этот метод для получения URL файла из кеша. |
| abstract [IsExisted](../../aspose.cells.gridjs/gridcacheforstream/isexisted/)(string) | Проверяет, существует ли кеш с uid |
| abstract [LoadStream](../../aspose.cells.gridjs/gridcacheforstream/loadstream/)(string) | Реализует этот метод для загрузки кеша по ключу uid, возвращает поток из кеша. |
| abstract [SaveStream](../../aspose.cells.gridjs/gridcacheforstream/savestream/)(Stream, string) | Реализует этот метод для сохранения кеша, сохраняет поток в кеш по ключу uid. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


