---
title: "ShapePropertyCollection.HasFormat3D"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ShapePropertyCollection-Methode. Gibt an, ob das Shape 3D-Formatdaten enthält"
type: docs
url: /de/net/aspose.cells.drawing/shapepropertycollection/hasformat3d/
---
## ShapePropertyCollection.HasFormat3D method

Gibt an, ob die Form 3D-Formatdaten enthält.

```csharp
public bool HasFormat3D()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCollectionMethodHasFormat3DDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("A2:A3", true);
            chart.NSeries.CategoryData = "B2:B3";

            // Auf 3D-Format prüfen
            Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            if (shapeProperties.HasFormat3D())
            {
                Format3D format3D = shapeProperties.Format3D;
                format3D.SurfaceLightingType = LightRigType.BrightRoom;
                format3D.LightingAngle = 30;
            }

            workbook.Save("HasFormat3DDemo.xlsx");
            Console.WriteLine("Workbook saved with 3D format demo.");
        }
    }
}
```

### Siehe auch

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


