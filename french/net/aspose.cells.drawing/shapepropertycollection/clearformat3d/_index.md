---
title: "ShapePropertyCollection.ClearFormat3D"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ShapePropertyCollection. Efface les propriétés de forme 3D de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapepropertycollection/clearformat3d/
---
## ShapePropertyCollection.ClearFormat3D method

Efface les propriétés de forme 3D de la forme.

```csharp
public void ClearFormat3D()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShapePropertyCollectionMethodClearFormat3DDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un graphique d'exemple
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);

            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // Accéder aux propriétés de forme de la première série
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Configurer le format 3D et le biseau
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Définir les couleurs des séries
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Enregistrez le classeur
            workbook.Save("ShapePropertyCollectionMethodClearFormat3DDemo.xlsx", SaveFormat.Xlsx);

            shapeProperties.ClearFormat3D();
            workbook.Save("ShapePropertyCollectionMethodClearFormat3DDemo2.xlsx", SaveFormat.Xlsx);

        }
    }
}
```

### Voir aussi

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


