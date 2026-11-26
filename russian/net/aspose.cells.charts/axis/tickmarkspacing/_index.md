---
title: "Axis.TickMarkSpacing"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Возвращает или задает количество категорий или серий между делениями. Применяется только к осям категорий и серий"
type: docs
url: /ru/net/aspose.cells.charts/axis/tickmarkspacing/
---
## Axis.TickMarkSpacing property

Возвращает или задает количество категорий или рядов между делениями. Применяется только к осям категорий и рядов.

```csharp
public int TickMarkSpacing { get; set; }
```

### Примечания

Число должно быть в диапазоне от 1 до 31999.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickMarkSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Добавить диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Настроить ось значений с помощью TickMarkSpacing
            Axis valueAxis = chart.ValueAxis;
            valueAxis.MinValue = 0;
            valueAxis.MaxValue = 200;
            valueAxis.MajorUnit = 25;
            valueAxis.MinorUnit = 5;
            valueAxis.TickMarkSpacing = 2; // Setting tick mark spacing
            
            // Настроить ось категорий с помощью TickMarkSpacing
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.TickMarkSpacing = 1; // Setting tick mark spacing

            workbook.Save("AxisTickMarkSpacingDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


