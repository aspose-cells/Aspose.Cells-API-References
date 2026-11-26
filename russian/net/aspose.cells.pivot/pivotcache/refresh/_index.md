---
title: "PivotCache.Refresh"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotCache. Обновляет данные из источника данных и вычисляет данные для представления всех PivotTable, чей источник данных — этот PivotCache."
type: docs
url: /ru/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот кэш сводных данных.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опция | PivotTableRefreshOption | Параметры обновления источника данных сводной таблицы. |

### Примечания

Лучше просто вызвать [`RefreshAll`](../../../aspose.cells/workbook/refreshall/), чтобы обновить все сводные таблицы и диаграммы в файле.

### См. также

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Обновляет данные из источника данных и вычисляет данные для представления всех сводных таблиц, чей источник данных — этот кэш сводных данных.

```csharp
public PivotRefreshState Refresh()
```

### Примечания

Если и table1, и table2 используют этот кэш, обе таблицы будут вычислены. Лучше просто вызвать [`RefreshAll`](../../../aspose.cells/workbook/refreshall/), чтобы обновить все сводные таблицы и диаграммы в файле.

### См. также

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


