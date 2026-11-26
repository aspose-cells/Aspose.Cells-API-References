---
title: "Marker.BackgroundColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Marker. Представляет цвет фона маркера в линейной диаграмме, точечной диаграмме или радиальной диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Представляет цвет фона маркера в линейной, точечной или радиальной диаграмме.

```csharp
public Color BackgroundColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);

            // Создать диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Настроить внешний вид маркера
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.Circle;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = System.Drawing.Color.Blue;
                series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
            }

            workbook.Save("MarkerBackgroundColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


