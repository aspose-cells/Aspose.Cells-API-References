---
title: "TickLabels.TickLabelItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels‑egenskap. Hämtar de visade tick‑etiketterna för axeln"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/ticklabelitems/
---
## TickLabels.TickLabelItems property

Hämtar de visade ticketiketterna för axeln.

```csharp
public TickLabelItem[] TickLabelItems { get; }
```

### Anmärkningar

Endast tillgänglig efter att ha anropat [`Calculate`](../../chart/calculate/)‑metoden.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTickLabelItemsDemo
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
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Beräkna diagrammet
            chart.Calculate();

            // Hämta kategori‑axeln och dess tick‑etiketter
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // Lägg till former för att markera varje tick-etikettposition
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // Lägg till en rektangel runt varje tick‑etikett
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;
            }

            // Spara arbetsboken
            workbook.Save("TickLabelItemsDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabelItem](../../ticklabelitem/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


