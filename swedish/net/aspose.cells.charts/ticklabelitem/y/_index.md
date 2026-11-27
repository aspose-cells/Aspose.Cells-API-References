---
title: "TickLabelItem.Y"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabelItem egenskap. Y-koordinater för Ticklabel‑objektet som en andel av diagramhöjden"
type: docs
url: /sv/net/aspose.cells.charts/ticklabelitem/y/
---
## TickLabelItem.Y property

Y-koordinater för Ticklabel-objektet som en andel av diagrammets höjd.

```csharp
public double Y { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelItemPropertyYDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            
            // Ställ in kategoriaxeldata med NSERIES istället för CategoryData
            chart.NSeries.CategoryData = "A1:A3";

            // Beräkna diagram för att säkerställa att tick‑etiketter genereras
            chart.Calculate();

            // Hämta tick‑etikettobjekt från kategoriaxeln
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = chart.CategoryAxis.TickLabels.TickLabelItems;

            // Demonstrera användning av Y‑egenskapen genom att lägga till former som är justerade med tick‑etiketter
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Lägg till en rektangel vid varje tick‑etiketts Y‑position
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y, // Using the Y property of TickLabelItem
                    item.X + 0.05, // Small width
                    item.Y + 0.02); // Small height
                
                shape.Fill.SolidFill.Color = Color.FromArgb(100, 0, 255, 0); // Semi-transparent green
                shape.Line.SolidFill.Color = Color.Black;
            }

            // Spara arbetsboken
            workbook.Save("TickLabelItemPropertyYDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


