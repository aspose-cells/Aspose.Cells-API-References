---
title: "Line.WeightPx"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Line. Получает или задает толщину линии в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Получает или задает толщину линии в пикселях.

```csharp
public double WeightPx { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPxDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Добавьте примерные данные
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Добавить линейную диаграмму
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Настройте свойства линии с WeightPx
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Сохраните книгу
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### См. также

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


