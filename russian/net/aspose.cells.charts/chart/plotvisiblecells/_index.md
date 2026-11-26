---
title: "Chart.PlotVisibleCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Chart. Указывает, следует ли строить только видимые ячейки"
type: docs
url: /ru/net/aspose.cells.charts/chart/plotvisiblecells/
---
## Chart.PlotVisibleCells property

Указывает, следует ли строить только видимые ячейки.

```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него используйте свойство PlotVisibleCellsOnly. Этот метод будет удалён через 12 месяцев, начиная с декабря 2022 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["A4"].PutValue("Eve");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(90);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(95);

            // Скрыть некоторые строки
            worksheet.Cells.HideRow(2);
            worksheet.Cells.HideRow(3);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Продемонстрировать свойство PlotVisibleCells
            chart.PlotVisibleCells = false; // Will not plot hidden cells
            // chart.PlotVisibleCells = true; // Будет строить скрытые ячейки (закомментировано для демонстрации)

            // Сохраните книгу
            workbook.Save("ChartPlotVisibleCellsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


