---
title: "ShapePropertyCollection.Format3D"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ShapePropertyCollection propriété. Représente un objet Format3D qui spécifie les propriétés de forme 3D pour l'élément de graphique ou la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapepropertycollection/format3d/
---
## ShapePropertyCollection.Format3D property

Représente un objet `Format3D` qui spécifie les propriétés de forme 3D pour l'élément de graphique ou la forme.

```csharp
public Format3D Format3D { get; }
```

### Exemples

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

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample 3D Chart");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Ajouter un histogramme à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:A4", false);

            // Accéder aux propriétés de forme des séries
            Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Appliquer le formatage 3D
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

### Voir aussi

* class [Format3D](../../format3d/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


