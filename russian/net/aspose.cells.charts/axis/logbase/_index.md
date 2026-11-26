---
title: "Axis.LogBase"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет логарифмическую основу. Значение по умолчанию — 10"
type: docs
url: /ru/net/aspose.cells.charts/axis/logbase/
---
## Axis.LogBase property

Представляет логарифмическую основу. Значение по умолчанию — 10.

```csharp
public double LogBase { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyLogBaseDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(Math.Pow(2, i-2)); // Exponential values
                worksheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить серию
            chart.NSeries.Add($"B2:B10", true);
            chart.NSeries[0].XValues = $"A2:A10";
            chart.NSeries[0].Name = "Logarithmic Series";

            // Настройте логарифмическую ось
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 2; // Set logarithmic base to 2
            chart.CategoryAxis.Title.Text = "Logarithmic Scale (Base 2)";
            
            // Сохраните книгу
            workbook.Save("AxisPropertyLogBaseDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


