---
title: "Format3D.SurfaceMaterialType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Format3D-Eigenschaft. Gibt den Materialtyp zurück und legt ihn fest, der mit den Beleuchtungseigenschaften kombiniert wird, um das endgültige Aussehen und Gefühl einer Form zu erzeugen. Standardwert ist PresetMaterialType.WarmMatte"
type: docs
url: /de/net/aspose.cells.drawing/format3d/surfacematerialtype/
---
## Format3D.SurfaceMaterialType property

Liest und setzt den Materialtyp, der mit den Beleuchtungseigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen. Standardwert ist PresetMaterialType.WarmMatte.

```csharp
public PresetMaterialType SurfaceMaterialType { get; set; }
```

### Beispiele

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

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);

            // Erstelle ein 3D-Säulendiagramm
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // 3D-Format-Eigenschaften konfigurieren
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

### Siehe auch

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


