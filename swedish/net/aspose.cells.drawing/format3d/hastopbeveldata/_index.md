---
title: "Format3D.HasTopBevelData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Format3D-metod. Anger om formen har toppramningsdata"
type: docs
url: /sv/net/aspose.cells.drawing/format3d/hastopbeveldata/
---
## Format3D.HasTopBevelData method

Indikerar om formen har data för övre fasning.

```csharp
public bool HasTopBevelData()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DMethodHasTopBevelDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Skapa 3D-diagram.
            int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Hämta 3D-format
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;

            // Ställ in toppramning
            format3D.TopBevel.Type = BevelPresetType.Circle;
            format3D.TopBevel.Width = 6;
            format3D.TopBevel.Height = 6;

            // Kontrollera och visa ramningsdata
            if (format3D.HasTopBevelData())
            {
                Console.WriteLine("Top Bevel Type: " + format3D.TopBevel.Type);
                Console.WriteLine("Top Bevel Width: " + format3D.TopBevel.Width);
                Console.WriteLine("Top Bevel Height: " + format3D.TopBevel.Height);
            }

            workbook.Save("Format3DTopBevelDemo.xlsx");
        }
    }
}
```

### Se även

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


