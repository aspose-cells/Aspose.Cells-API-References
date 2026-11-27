---
title: "Klass Bevel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Bevel-klass. Representerar en avfasning av en form"
type: docs
url: /sv/net/aspose.cells.drawing/bevel/
---
## Bevel class

Representerar en fasning av en form

```csharp
public class Bevel
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Hämtar och anger höjden på avfasningen, eller hur långt ovanför formen den tillämpas. I enheten punkter. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Hämtar och anger den förinställda avfasningstypen. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Hämtar och anger bredden på avfasningen, eller hur djupt in i formen den tillämpas. I enheten punkter. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till dataserier i diagrammet
            chart.NSeries.Add("A1:B4", true);

            // Åtkomst till diagrammets plotområde
            ChartFrame plotArea = chart.PlotArea;

            // Kom åt formegenskaperna för diagramområdet
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Kom åt 3D-formatets egenskaper
            Format3D format3D = shapeProperties.Format3D;

            // Kom åt egenskaperna för den övre fasningen
            Bevel topBevel = format3D.TopBevel;

            // Ställ in bredd, höjd och typ för avfasen
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Ställ in andra 3D-formategenskaper
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Spara arbetsboken
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


