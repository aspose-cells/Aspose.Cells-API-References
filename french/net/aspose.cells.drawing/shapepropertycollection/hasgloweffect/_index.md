---
title: "ShapePropertyCollection.HasGlowEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ShapePropertyCollection méthode. Indique si la forme possède des données d'effet de lueur"
type: docs
url: /fr/net/aspose.cells.drawing/shapepropertycollection/hasgloweffect/
---
## ShapePropertyCollection.HasGlowEffect method

Indique si la forme possède des données d'effet de lueur.

```csharp
public bool HasGlowEffect()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;
    using System;

    public class ShapePropertyCollectionMethodHasGlowEffectDemo
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

            GlowEffect glowEffect = shapeProperties.GlowEffect;
            glowEffect.Size = 30;
            glowEffect.Color.Color = Color.Red;

            Console.WriteLine("Shape has glow effect: " + shapeProperties.HasGlowEffect());
                       

            // Enregistrer le résultat
            workbook.Save("ShapePropertyCollectionMethodHasGlowEffectDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


