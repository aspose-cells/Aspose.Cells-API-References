---
title: "Axis.IsLogarithmic"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет, является ли тип шкалы оси значений логарифмическим или нет"
type: docs
url: /ru/net/aspose.cells.charts/axis/islogarithmic/
---
## Axis.IsLogarithmic property

Представляет, является ли тип шкалы оси значений логарифмическим.

```csharp
public bool IsLogarithmic { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsLogarithmicDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(100);
            worksheet.Cells["A4"].PutValue(1000);
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(100);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавить серию
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries[0].Values = "B1:B4";

            // Настройте логарифмическую ось
            chart.CategoryAxis.IsLogarithmic = true;
            chart.CategoryAxis.LogBase = 10;
            chart.CategoryAxis.MinValue = 1;
            chart.CategoryAxis.MaxValue = 10000;

            // Сохраните книгу
            workbook.Save("AxisPropertyIsLogarithmicDemo_out.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


