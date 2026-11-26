---
title: "Series.HasDropLines"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Истина, если диаграмма имеет линии спуска. Применяется только к линейным или областным диаграммам."
type: docs
url: /ru/net/aspose.cells.charts/series/hasdroplines/
---
## Series.HasDropLines property

Истина, если у диаграммы есть линии падения. Применяется только к линейным или областным диаграммам.

```csharp
public bool HasDropLines { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasDropLinesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавить линейную диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить данные серии
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию
            Series series = chart.NSeries[0];

            // Продемонстрировать свойство HasDropLines
            series.HasDropLines = true; // Enable drop lines
            series.Type = ChartType.Line; // Ensure it's a line chart for drop lines to be visible

            // Сохраните книгу
            workbook.Save("SeriesHasDropLinesDemo.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


