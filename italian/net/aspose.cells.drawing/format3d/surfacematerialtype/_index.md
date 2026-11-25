---
title: "Format3D.SurfaceMaterialType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Format3D. Ottiene e imposta il tipo di materiale che, combinato con le proprietà di illuminazione, conferisce l'aspetto finale a una forma. Il valore predefinito è PresetMaterialType.WarmMatte"
type: docs
url: /it/net/aspose.cells.drawing/format3d/surfacematerialtype/
---
## Format3D.SurfaceMaterialType property

Ottiene e imposta il tipo di materiale che, combinato con le proprietà di illuminazione, conferisce l'aspetto finale a una forma. Il valore predefinito è PresetMaterialType.WarmMatte.

```csharp
public PresetMaterialType SurfaceMaterialType { get; set; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);

            // Crea un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Configura le proprietà del formato 3D
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

### Vedi anche

* enum [PresetMaterialType](../../presetmaterialtype/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


