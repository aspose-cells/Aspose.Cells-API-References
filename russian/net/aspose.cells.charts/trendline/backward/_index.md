---
title: "Trendline.Backward"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Возвращает или задает количество периодов или единиц на диаграмме рассеяния, на которое трендовая линия расширяется назад. Количество периодов должно быть больше или равно нулю. Если тип диаграммы — столбчатая, количество периодов должно быть в диапазоне от 0 до 0,5."
type: docs
url: /ru/net/aspose.cells.charts/trendline/backward/
---
## Trendline.Backward property

Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое линия тренда расширяется назад. Количество периодов должно быть больше или равно нулю. Если тип диаграммы — столбчатая, количество периодов должно быть от 0 до 0,5.

```csharp
public double Backward { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);

            // Добавьте трендовую линию и получите её по индексу
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(Aspose.Cells.Charts.TrendlineType.Linear);
            Aspose.Cells.Charts.Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            trendline.Name = "Linear Trend";
            trendline.DisplayEquation = true;
            
            // Установите свойство backward, чтобы расширить трендовую линию назад на 0,5 единицы
            trendline.Backward = 0.5;
            
            workbook.Save("TrendlineBackwardDemo.xlsx");
        }
    }
}
```

### См. также

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


