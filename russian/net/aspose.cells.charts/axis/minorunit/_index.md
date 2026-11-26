---
title: "Axis.MinorUnit"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Axis. Представляет минорные единицы для оси"
type: docs
url: /ru/net/aspose.cells.charts/axis/minorunit/
---
## Axis.MinorUnit property

Представляет вспомогательные единицы для оси.

```csharp
public double MinorUnit { get; set; }
```

### Примечания

Минорные единицы должны быть больше нуля.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinorUnitDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Добавьте примерные данные
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Настройте данные диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Настроить ось значений
            chart.ValueAxis.Title.Text = "Sales Amount";
            chart.ValueAxis.MajorUnit = 20000;
            chart.ValueAxis.MinorUnit = 5000; // Demonstrate MinorUnit property
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 80000;

            // Сохраните книгу
            workbook.Save("AxisPropertyMinorUnitDemo.xlsx");
        }
    }
}
```

### См. также

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


