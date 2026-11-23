---
title: "ShadowEffect.Distance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShadowEffect. Obtient et définit la distance de l'ombre. Plage de 0 à 200 points"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Obtient et définit la distance de l'ombre. Plage de 0 à 200 points.

```csharp
public double Distance { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyDistanceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 150, 100);
            
            // Configurer l'effet d'ombre
            ShadowEffect shadow = rectangle.ShadowEffect;
            shadow.PresetType = PresetShadowType.OffsetDiagonalTopRight;
            
            // Créer un objet CellsColor et définir les valeurs ARGB
            CellsColor color = workbook.CreateCellsColor();
            color.Argb = (128 << 24) | (255 << 16) | (0 << 8) | 0; // Semi-transparent red
            shadow.Color = color;
            
            shadow.Transparency = 0.3;
            shadow.Blur = 15;
            shadow.Angle = 45;
            shadow.Distance = 20; // Set distance to 20 points

            // Afficher la distance de l'ombre
            Console.WriteLine("Shadow Distance: " + shadow.Distance + " points");

            // Enregistrer le classeur avec l'effet d'ombre
            workbook.Save("ShadowEffectPropertyDistanceDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


