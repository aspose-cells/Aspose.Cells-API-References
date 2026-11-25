---
title: "ShapePropertyCollection.Format3D"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ShapePropertyCollection. Rappresenta un oggetto Format3D che specifica le proprietà della forma 3D per l'elemento del grafico o la forma"
type: docs
url: /it/net/aspose.cells.drawing/shapepropertycollection/format3d/
---
## ShapePropertyCollection.Format3D property

Rappresenta un oggetto `Format3D` che specifica le proprietà della forma 3D per l'elemento del grafico o la forma.

```csharp
public Format3D Format3D { get; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample 3D Chart");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Aggiungi grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", false);

            // Accedi alle proprietà della forma della serie
            Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Applica formattazione 3D
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

### Vedi anche

* class [Format3D](../../format3d/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


