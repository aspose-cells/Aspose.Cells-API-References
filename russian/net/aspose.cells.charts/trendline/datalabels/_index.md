---
title: "Trendline.DataLabels"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Trendline. Представляет объект DataLabels для указанной серии."
type: docs
url: /ru/net/aspose.cells.charts/trendline/datalabels/
---
## Trendline.DataLabels property

Представляет объект DataLabels для указанного ряда.

```csharp
public DataLabels DataLabels { get; }
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
    public class TrendlinePropertyDataLabelsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Создать диаграмму
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Добавьте серию и задайте линию тренда.
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");

            // Настройте DataLabels для линии тренда.
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Red;
            trendline.DataLabels.Font.IsBold = true;
            trendline.DataLabels.Position = LabelPositionType.Above;
            trendline.DataLabels.Border.IsVisible = true;
            trendline.DataLabels.Border.Color = Color.Black;

            // Сохраните книгу
            workbook.Save("TrendlineDataLabelsDemo.xlsx");
        }
    }
}
```

### См. также

* class [DataLabels](../../datalabels/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


