---
title: "Klass TickLabelItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.TickLabelItem klass. Representerar en tick-etikett i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Representerar en tick‑etikett i diagrammet.

```csharp
public class TickLabelItem
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Höjd på Ticklabel-objektet som en andel av diagrammets höjd. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Bredd på Ticklabel-objektet som en andel av diagrammets bredd. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | X-koordinater för Ticklabel-objektet som en andel av diagrammets bredd. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Y-koordinater för Ticklabel-objektet som en andel av diagrammets höjd. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet
            chart.Calculate();

            // Åtkomst till kategoriaxelns tick-etiketter
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Lägg till former för att markera varje tick-etikettposition
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Lägg till en rektangel runt tick-etiketten
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // Lägg till en cirkel bredvid tick-etiketten
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Spara arbetsboken
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


