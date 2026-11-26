---
title: "Format3D.SurfaceLightingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Format3D. Obtiene y establece el tipo de iluminación que se aplicará a la escena de la forma. El valor predeterminado es LightRigType.ThreePoint"
type: docs
url: /es/net/aspose.cells.drawing/format3d/surfacelightingtype/
---
## Format3D.SurfaceLightingType property

Obtiene y establece el tipo de iluminación que se aplicará a la escena de la forma. El valor predeterminado es LightRigType.ThreePoint.

```csharp
public LightRigType SurfaceLightingType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DPropertySurfaceLightingTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(8);
            worksheet.Cells["A4"].PutValue(12);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", true);

            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;

            format3D.SurfaceMaterialType = PresetMaterialType.Plastic;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 30;

            workbook.Save("Format3DPropertySurfaceLightingTypeDemo.xlsx");
            Console.WriteLine("3D chart with SurfaceLightingType set created successfully.");
        }
    }
}
```

### Ver también

* enum [LightRigType](../../lightrigtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


