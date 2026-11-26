---
title: "Trendline.DisplayRSquared"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Указывает, отображается ли значение Rsquared трендовой линии на диаграмме в той же подписи данных, что и уравнение. Установка этого свойства в значение True автоматически включает подписи данных."
type: docs
url: /ru/net/aspose.cells.charts/trendline/displayrsquared/
---
## Trendline.DisplayRSquared property

Отображает, отображается ли значение R‑квадрата линии тренда на диаграмме (в той же подписи данных, что и уравнение). Установка этого свойства в True автоматически включает подписи данных.

```csharp
public bool DisplayRSquared { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayRSquaredDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(4);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(8);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Добавьте трендовую линию и получите её по индексу
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            
            // Продемонстрировать свойство DisplayRSquared
            trendline.DisplayRSquared = true;
            trendline.DisplayEquation = true;

            // Сохраните книгу
            workbook.Save("TrendlineDisplayRSquaredDemo.xlsx");
        }
    }
}
```

### См. также

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


