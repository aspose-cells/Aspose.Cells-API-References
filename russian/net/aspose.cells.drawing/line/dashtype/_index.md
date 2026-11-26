---
title: "Line.DashType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает тип пунктирной линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/dashtype/
---
## Line.DashType property

Указывает тип пунктирной линии

```csharp
public MsoLineDashStyle DashType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyDashTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Настройте тип штриха линии серии
            chart.CategoryAxis.MajorGridLines.DashType = MsoLineDashStyle.DashDot;
            chart.CategoryAxis.MinorGridLines.DashType = MsoLineDashStyle.DashLongDashDot;

            // Настройте линию серии
            chart.NSeries[0].Border.DashType = MsoLineDashStyle.Solid;
            chart.NSeries[0].Border.Color = System.Drawing.Color.Blue;

            workbook.Save("LineDashTypeDemo.xlsx");
            Console.WriteLine("Line chart with custom dash types created successfully.");
        }
    }
}
```

### См. также

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


