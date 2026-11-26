---
title: "Line.EndArrowWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Указывает ширину наконечника стрелки для конца линии"
type: docs
url: /ru/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

Указывает ширину наконечника стрелки для конца линии.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowWidthDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для линейной диаграммы
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Добавить линейную диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установите источник данных диаграммы
            chart.NSeries.Add("A1:B3", true);

            // Настройте свойства линии для первой серии
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // Сохраните книгу
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### См. также

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


