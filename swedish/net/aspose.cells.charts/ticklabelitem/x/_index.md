---
title: "TickLabelItem.X"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabelItem egenskap. X-koordinater för Ticklabel‑objektet som en andel av diagrambredden"
type: docs
url: /sv/net/aspose.cells.charts/ticklabelitem/x/
---
## TickLabelItem.X property

X-koordinater för Ticklabel-objektet som en andel av diagrammets bredd.

```csharp
public double X { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyXDemo
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

            // Lägg till former vid varje tick‑etikettposition med X‑egenskapen
            for (int i = 0; i < items.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = items[i];
                
                // Lägg till rektangel vid tick‑etikettposition
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X, 
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Color = Color.LightBlue;
                shape.Line.SolidFill.Color = Color.Blue;

                // Lägg till cirkel bredvid tick‑etiketten med X‑egenskapen
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + 0.05, // Small offset
                    item.Y + item.Height);
                
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // Spara arbetsboken
            workbook.Save("TickLabelItemPropertyXDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


