---
title: "Trendline.DisplayEquation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Определяет, отображается ли уравнение линии тренда на диаграмме в той же метке данных, что и значение R‑квадрат. Установка этого свойства в True автоматически включает метки данных."
type: docs
url: /ru/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Отображает, отображается ли уравнение линии тренда на диаграмме (в той же подписи данных, что и значение R‑квадрата). Установка этого свойства в True автоматически включает подписи данных.

```csharp
public bool DisplayEquation { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавьте серию и линию тренда.
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Настройте свойства линии тренда.
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### См. также

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


