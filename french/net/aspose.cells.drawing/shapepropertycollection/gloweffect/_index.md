---
title: "ShapePropertyCollection.GlowEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ShapePropertyCollection propriété. Représente un objet GlowEffect qui spécifie l'effet de lueur pour l'élément de graphique ou la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shapepropertycollection/gloweffect/
---
## ShapePropertyCollection.GlowEffect property

Représente un objet `GlowEffect` qui spécifie l'effet de lueur pour l'élément de graphique ou la forme.

```csharp
public GlowEffect GlowEffect { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShapePropertyCollectionPropertyGlowEffectDemo
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

            // Définir les couleurs des séries
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Enregistrez le classeur
            workbook.Save("GlowEffectDemo.xlsx");            
        }
    }
}
```

### Voir aussi

* class [GlowEffect](../../gloweffect/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


