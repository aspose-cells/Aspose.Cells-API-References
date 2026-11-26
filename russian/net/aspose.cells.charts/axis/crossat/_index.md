---
title: "Axis.CrossAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет точку на оси значений, где пересекается категориальная ось"
type: docs
url: /ru/net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Представляет точку на оси значений, где пересекает её ось категорий.

```csharp
public double CrossAt { get; set; }
```

### Примечания

Число должно быть целым, когда оно применяется к категориальной оси. И значение должно быть между 1 и 31999.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossAtDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Настроить ось значений
            chart.ValueAxis.CrossAt = 15; // Cross at value 15
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 50;

            // Настроить категориальную ось
            chart.CategoryAxis.CrossAt = 2.5; // Cross between categories B and C
            chart.CategoryAxis.TickLabelPosition = Aspose.Cells.Charts.TickLabelPositionType.Low;

            // Сохраните книгу
            workbook.Save("AxisCrossAtDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


