---
title: "TickLabelItem.Width"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabelItem egenskap. Bredd på Ticklabel‑objektet som en andel av diagrambredden"
type: docs
url: /sv/net/aspose.cells.charts/ticklabelitem/width/
---
## TickLabelItem.Width property

Bredd på Ticklabel-objektet som en andel av diagrammets bredd.

```csharp
public double Width { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyWidthDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet
            chart.Calculate();

            // Åtkomst till tick‑etikettobjekt
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] items = axis.TickLabels.TickLabelItems;

            // Demonstrera Width‑egenskapen genom att lägga till former som matchar tick‑etikettens dimensioner
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Lägg till rektangel som matchar tick label dimensions (med Width property)
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Spara arbetsboken
            workbook.Save("TickLabelItemWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


