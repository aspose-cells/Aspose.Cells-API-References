---
title: "Line.JoinType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает тип соединительных концов"
type: docs
url: /ru/net/aspose.cells.drawing/line/jointype/
---
## Line.JoinType property

Указывает соединительные концы.

```csharp
public LineJoinType JoinType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyJoinTypeDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Установите тип соединения линии
            Line majorGridLines = chart.ValueAxis.MajorGridLines;
            majorGridLines.JoinType = LineJoinType.Round;

            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### См. также

* enum [LineJoinType](../../linejointype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


