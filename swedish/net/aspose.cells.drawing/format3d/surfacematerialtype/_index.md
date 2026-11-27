---
title: "Format3D.SurfaceMaterialType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Format3D‑egenskap. Hämtar och anger materialtypen som kombineras med belysningsegenskaperna för att ge formen ett slutgiltigt utseende och känsla. Standardvärdet är PresetMaterialType.WarmMatte"
type: docs
url: /sv/net/aspose.cells.drawing/format3d/surfacematerialtype/
---
## Format3D.SurfaceMaterialType property

Hämtar och anger materialtypen som kombineras med belysningsegenskaperna för att ge en form dess slutgiltiga utseende och känsla. Standardvärdet är PresetMaterialType.WarmMatte.

```csharp
public PresetMaterialType SurfaceMaterialType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DPropertySurfaceMaterialTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);

            // Skapa 3D kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Konfigurera 3D-formategenskaper
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;
            format3D.LightingAngle = 30;
            format3D.SurfaceLightingType = LightRigType.BrightRoom;

            workbook.Save("Format3DPropertySurfaceMaterialTypeDemo.xlsx");
            Console.WriteLine("Workbook saved with 3D chart using Metal surface material.");
        }
    }
}
```

### Se även

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


