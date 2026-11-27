---
title: "TickLabelItem.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabelItem‑egenskap. Höjd på Ticklabel‑objektet som en kvot av diagrammets höjd"
type: docs
url: /sv/net/aspose.cells.charts/ticklabelitem/height/
---
## TickLabelItem.Height property

Höjd på Ticklabel-objektet som en andel av diagrammets höjd.

```csharp
public double Height { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyHeightDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet
            chart.Calculate();

            // Åtkomst till kategoriaxelns tick-etiketter
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Lägg till former för att visualisera tick label item‑höjder
            foreach (TickLabelItem item in tickLabelItems)
            {
                // Lägg till rektangel som visar gränserna för tick label item
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;

                // Lägg till text som visar höjdvärdet
                Shape textShape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.TextBox,
                    PlacementType.Move,
                    item.X,
                    item.Y - 0.05, // Position above the tick label
                    0.1,
                    0.05);
                
                textShape.Text = $"H: {item.Height:F4}";
                textShape.Fill.SolidFill.Transparency = 1;
            }

            // Spara arbetsboken
            workbook.Save("TickLabelItemHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


