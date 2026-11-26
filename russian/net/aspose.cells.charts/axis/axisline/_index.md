---
title: "Axis.AxisLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Получает внешний вид оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

Получает внешний вид оси.

```csharp
public Line AxisLine { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisLineDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Установите источник данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Доступ к оси значений
            Axis valueAxis = chart.ValueAxis;

            // Настроить свойства линии оси
            valueAxis.AxisLine.Color = Color.Red;
            valueAxis.AxisLine.Style = LineType.DashDot;
            valueAxis.AxisLine.Weight = WeightType.MediumLine;

            // Сохраните книгу
            workbook.Save("AxisLineDemo.xlsx");
        }
    }
}
```

### См. также

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


