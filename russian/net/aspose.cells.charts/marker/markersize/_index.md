---
title: "Marker.MarkerSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Marker. Представляет размер маркера в единицах точек. Применяется к линейной диаграмме, точечной диаграмме или радиальной диаграмме"
type: docs
url: /ru/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Представляет размер маркера в единицах пунктов. Применяется к линейной диаграмме, точечной диаграмме или радиальной диаграмме.

```csharp
public int MarkerSize { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Добавьте серию — исправленный вызов метода
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // Установить свойства маркера
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Сохраните книгу
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


