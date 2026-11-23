---
title: "Classe GlowEffect"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.GlowEffect. Cette classe spécifie un effet de lueur dans lequel un contour flou de couleur est ajouté à l'extérieur des bords de l'objet"
type: docs
url: /fr/net/aspose.cells.drawing/gloweffect/
---
## GlowEffect class

Cette classe spécifie un effet de lueur, dans lequel un contour flou de couleur est ajouté à l'extérieur des bords de l'objet.

```csharp
public class GlowEffect
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Color](../../aspose.cells.drawing/gloweffect/color/) { get; set; } | Obtient la couleur de l'effet de lueur. |
| [Radius](../../aspose.cells.drawing/gloweffect/radius/) { get; set; } | (**Obsolète.**) Obtient et définit le rayon de la lueur, en unité de points. |
| [Size](../../aspose.cells.drawing/gloweffect/size/) { get; set; } | Obtient et définit le rayon de la lueur, en unité de points. |
| [Transparency](../../aspose.cells.drawing/gloweffect/transparency/) { get; set; } | Obtient et définit le degré de transparence de l'effet de lueur. Plage de 0,0 (opaque) à 1,0 (transparent). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GlowEffectDemo
    {
        public static void GlowEffectExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme d'arc à la feuille de calcul
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Définir le placement de l'arc
            arcShape.Placement = PlacementType.FreeFloating;

            // Définir le format de remplissage
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Définir le style de ligne
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Créer une instance de GlowEffect et définir ses propriétés
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Enregistrez le classeur
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


