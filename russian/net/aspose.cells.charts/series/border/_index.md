---
title: "Series.Border"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Series. Представляет границу объекта Series"
type: docs
url: /ru/net/aspose.cells.charts/series/border/
---
## Series.Border property

Представляет границу объекта Series.

```csharp
public Line Border { get; }
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
    public class SeriesPropertyBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["A2"].PutValue("2020");
            worksheet.Cells["A3"].PutValue("2021");
            worksheet.Cells["A4"].PutValue("2022");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(7000);
            worksheet.Cells["B4"].PutValue(9000);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Добавить данные серии
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Получить первую серию
            Series series = chart.NSeries[0];
            series.Name = "Sales Data";

            // Настроить свойства границы
            series.Border.Color = System.Drawing.Color.Blue;
            series.Border.Weight = WeightType.MediumLine;
            series.Border.DashType = MsoLineDashStyle.Solid;
            series.Border.IsVisible = true;

            // Сохраните книгу
            workbook.Save("SeriesBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


