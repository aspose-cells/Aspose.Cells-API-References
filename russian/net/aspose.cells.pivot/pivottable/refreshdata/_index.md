---
title: "PivotTable.RefreshData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Обновляет данные из её источника данных в кэш сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Обновляет данные из её источника данных в кэш сводной таблицы.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Примечания

Мы соберём данные из источника данных в кэш сводных таблиц, затем вычислим данные из кэша в ячейки. И лучше, если вы просто вызовете [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) чтобы обновить и вычислить все сводные таблицы в файле, а не обновлять их по одной. ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод [`Refresh`](../../pivotcache/refresh/) и удалите последующий [`CalculateData`](../calculatedata/), потому что эта сводная таблица будет вычислена при обновлении [`PivotCache`](../pivotcache/). Этот метод будет удалён через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Создать сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Добавьте строки и поля данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Обновить и вычислить данные сводной таблицы
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Сохраните книгу
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Обновляет данные и настройки сводной таблицы из её источника данных с параметрами.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опция | PivotTableRefreshOption | Параметры обновления источника данных сводной таблицы. |

### Примечания

Мы соберём данные из источника данных в кэш сводных таблиц, затем вычислим данные из кэша в ячейки. И лучше, если вы просто вызовете [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) чтобы обновить и вычислить все сводные таблицы в файле, а не обновлять их по одной. ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод [`Refresh`](../../pivotcache/refresh/) и удалите последующий [`CalculateData`](../calculatedata/), потому что эта сводная таблица будет вычислена при обновлении [`PivotCache`](../pivotcache/). Этот метод будет удалён через 12 месяцев, начиная с июня 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("example.xlsx");
            
            // Получить доступ к листу, содержащему сводную таблицу
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Получить первую сводную таблицу на листе
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Настроить параметры обновления
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Обновить данные сводной таблицы с указанными параметрами
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Сохранить изменённую книгу
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### См. также

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


