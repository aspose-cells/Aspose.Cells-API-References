---
title: "Bevel.Height"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Bevel egenskap. Hämtar och anger höjden på avfasningen eller hur långt ovanför formen den tillämpas. I enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/bevel/height/
---
## Bevel.Height property

Hämtar och anger höjden på avfasningen, eller hur långt ovanför formen den tillämpas. I enheten punkter.

```csharp
public double Height { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class BevelPropertyHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(1500);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Åtkomst till plotområdets 3D-format
            Format3D format3D = chart.PlotArea.ShapeProperties.Format3D;

            // Konfigurera övre avfasning med Height‑egenskapen
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.ArtDeco;
            topBevel.Width = 8;
            topBevel.Height = 4.5; // Demonstrating Height property usage

            // Spara arbetsboken
            workbook.Save("BevelHeightDemo.xlsx");
        }
    }
}
```

### Se även

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


