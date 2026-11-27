---
title: "ShapePropertyCollection.Format3D"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePropertyCollection egenskap. Representerar ett Format3D-objekt som specificerar 3D-formegenskaper för diagrammet eller formen"
type: docs
url: /sv/net/aspose.cells.drawing/shapepropertycollection/format3d/
---
## ShapePropertyCollection.Format3D property

Representerar ett `Format3D`-objekt som specificerar 3D-formegenskaper för diagrammet eller formen.

```csharp
public Format3D Format3D { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCollectionPropertyFormat3DDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample 3D Chart");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Lägg till 3D-stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", false);

            // Kom åt seriernas formegenskaper
            Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Tillämpa 3D-formatering
            Format3D format3D = shapeProperties.Format3D;
            format3D.SurfaceLightingType = LightRigType.BrightRoom;
            format3D.LightingAngle = 30;
            format3D.TopBevel.Type = BevelPresetType.ArtDeco;
            format3D.TopBevel.Height = 8;
            format3D.TopBevel.Width = 8;

            workbook.Save("Format3DDemo.xlsx");
            Console.WriteLine("3D formatting applied and saved to Format3DDemo.xlsx");
        }
    }
}
```

### Se även

* class [Format3D](../../format3d/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


