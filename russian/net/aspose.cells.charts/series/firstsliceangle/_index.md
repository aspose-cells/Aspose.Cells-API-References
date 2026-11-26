---
title: "Series.FirstSliceAngle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Получает или задает угол первого сектора круговой или кольцевой диаграммы в градусах по часовой стрелке от вертикали. Применяется только к круговым, 3D‑круговым и кольцевым диаграммам со значениями от 0 до 360"
type: docs
url: /ru/net/aspose.cells.charts/series/firstsliceangle/
---
## Series.FirstSliceAngle property

Получает или задает угол первого сектора круговой или кольцевой диаграммы в градусах (по часовой стрелке от вертикали). Применяется только к круговым, 3‑D круговым и кольцевым диаграммам, значения от 0 до 360.

```csharp
public short FirstSliceAngle { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для диаграммы pie.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Добавить круговую диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию и установить FirstSliceAngle
            Series series = chart.NSeries[0];
            series.FirstSliceAngle = 45; // Rotate pie chart by 45 degrees

            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### См. также

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


