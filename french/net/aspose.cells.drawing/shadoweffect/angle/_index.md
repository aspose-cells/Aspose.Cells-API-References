---
title: "ShadowEffect.Angle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ShadowEffect. Obtient et définit l'angle d'éclairage. Plage de 0 à 359,9 degrés"
type: docs
url: /fr/net/aspose.cells.drawing/shadoweffect/angle/
---
## ShadowEffect.Angle property

Obtient et définit l'angle d'éclairage. Plage de 0 à 359,9 degrés.

```csharp
public double Angle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShadowEffectPropertyAngleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme et définir l'angle de l'effet d'ombre
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.ShadowEffect.Angle = 45;

            // Vérifier et afficher la valeur de l'angle
            Console.WriteLine("Shadow Effect Angle: " + shape.ShadowEffect.Angle);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


