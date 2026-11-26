---
title: "Axis.MinValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет минимальное значение на оси значений"
type: docs
url: /ru/net/aspose.cells.charts/axis/minvalue/
---
## Axis.MinValue property

Представляет минимальное значение на оси значений.

```csharp
public object MinValue { get; set; }
```

### Примечания

Тип minValue может быть только double или DateTime

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите доступ к первому листу и добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(40);
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(60);

            // Добавить диаграмму и задать диапазон данных
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", false);

            // Настроить свойства оси значений
            chart.ValueAxis.MinValue = 15;  // Setting minimum value
            chart.ValueAxis.MaxValue = 70;
            chart.ValueAxis.MajorUnit = 10;

            // Сохраните книгу
            workbook.Save("AxisMinValueDemo.xlsx");

            Console.WriteLine("Chart created with MinValue set to 15.");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


