---
title: "Klass Format3D"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Format3D-klass. Denna klass specificerar 3D-formegenskaperna för ett diagramelement eller en form"
type: docs
url: /sv/net/aspose.cells.drawing/format3d/
---
## Format3D class

Denna klass specificerar 3D-formegenskaper för ett diagramelement eller en form.

```csharp
public class Format3D
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Hämtar och anger belysningsvinkeln. Omfång från 0 till 359,9 grader. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Hämtar och anger belysningstypen som ska tillämpas på formens scen. Standardvärdet är LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Hämtar och anger materialtypen som kombineras med belysningsegenskaperna för att ge en form dess slutgiltiga utseende och känsla. Standardvärdet är PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Hämtar [`Bevel`](../bevel/)‑objektet som innehåller egenskaperna för att definiera en fasning på formens övre eller främre yta. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Indikerar om formen har data för övre fasning. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            chart.NSeries.Add("A1:A4", true);

            // Åtkomst till den första serien
            Series series = chart.NSeries[0];

            // Få åtkomst till seriens 3D-format
            Format3D format3D = series.ShapeProperties.Format3D;

            // Ange 3D-formatets egenskaper
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Kontrollera om formen har data för övre fasning
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Spara arbetsboken
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


