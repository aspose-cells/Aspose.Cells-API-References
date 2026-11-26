---
title: "PivotTable.PreserveFormatting"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, сохраняется ли форматирование ячеек PivotTableFormat при обновлении или перерасчёте PivotTable"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Указывает, сохраняется ли форматирование ячеек ([`PivotTableFormat`](../../pivottableformat/)) при обновлении или перерасчёте PivotTable.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него используйте свойство PivotTable.PreserveCellFormattingOnUpdate. Этот метод будет удалён через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook("source.xlsx");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к первой сводной таблице.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Включить сохранение форматирования при обновлении
            pivotTable.PreserveFormatting = true;
            
            // Применить некоторое форматирование к области данных сводной таблицы
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Отформатировать область данных сводной таблицы
            pivotTable.FormatAll(style);
            
            // Обновить и вычислить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


