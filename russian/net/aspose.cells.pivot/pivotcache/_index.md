---
title: "Класс PivotCache"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Pivot.PivotCache класс. Представляет кэш памяти для некоторых отчетов PivotTable."
type: docs
url: /ru/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

Представляет кэш памяти для некоторых отчетов PivotTable.

```csharp
public abstract class PivotCache : IDisposable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | Получает и задает количество неиспользуемых элементов, допускаемых до их удаления. Это значение ДОЛЖНО быть больше -2 и меньше 1048577. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | Получает [`PivotTableSourceType`](../pivottablesourcetype/). |

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | Освободите все ресурсы. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | Получает все сводные таблицы с этим кэшем сводных данных. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот кэш сводных данных. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот кэш сводных данных. |

### Примечания

Все данные будут собраны в этом кэше, и сводная таблица будет получать данные только из этого кэша, а не обращаться напрямую к источнику данных. Если источник данных некоторых [`PivotTable`](../pivottable/) одинаковый, они будут использовать общий кэш сводных данных.

### См. также

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


