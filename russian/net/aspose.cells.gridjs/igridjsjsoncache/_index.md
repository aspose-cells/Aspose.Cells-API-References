---
title: "Интерфейс IGridJsJsonCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.GridJs.IGridJsJsonCache. Интерфейс JSON‑кэша, который клиенты реализуют для конкретных стратегий хранения и инвалидирования."
type: docs
url: /ru/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

Интерфейс кэша JSON — клиенты реализуют конкретные стратегии хранения и инвалидирования.

```csharp
public interface IGridJsJsonCache
```

## Методы

| Имя | Описание |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | Очистить все кэши |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | Создать ключ кэша. Клиенты могут решить, включать ли uid в зависимости от бизнес‑требований. - Если важен только имя файла: игнорировать uid и использовать только fileName (рекомендовано, позволяет делиться кэшем между одинаковыми файлами). - Если необходимо различать файлы с одинаковым именем: использовать uid (строгий режим). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | Аннулировать указанную запись кэша. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | Аннулировать все записи кэша, содержащие указанный uid. Это полезно, когда вы не знаете точное значение fileName, используемое для кэширования. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | Записать JSON в кэш. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | Попытка получить JSON из кэша. |

### См. также

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


