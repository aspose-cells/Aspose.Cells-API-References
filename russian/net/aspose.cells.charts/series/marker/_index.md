---
title: "Series.Marker"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Возвращает маркер"
type: docs
url: /ru/net/aspose.cells.charts/series/marker/
---
## Series.Marker property

Возвращает `marker`.

```csharp
public Marker Marker { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyMarkerDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Настройте свойства маркера
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.SquarePlus;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = Color.Red;
                series.Marker.BackgroundColor = Color.Yellow;
            }

            workbook.Save("SeriesMarkerDemo.xlsx");
        }
    }
}
```

### См. также

* class [Marker](../../marker/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


