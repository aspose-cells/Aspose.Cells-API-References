---
title: "GradientFill.Angle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientFill. L'angle du remplissage linéaire"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/angle/
---
## GradientFill.Angle property

L'angle du remplissage linéaire.

```csharp
public float Angle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyAngleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme pour démontrer le remplissage en dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Définir les propriétés de remplissage de dégradé
            shape.Fill.FillType = FillType.Gradient;
            shape.Fill.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromCenter);
            shape.Fill.GradientFill.Angle = 45; // Set the angle to 45 degrees

            // Définir les couleurs du dégradé
            shape.Fill.GradientFill.SetTwoColorGradient(
                Color.Red, 
                Color.Blue, 
                GradientStyleType.Horizontal, 
                1);

            // Enregistrez le classeur
            workbook.Save("GradientFillAngleDemo.xlsx");

            Console.WriteLine("Demo completed. File saved with gradient fill at 45 degree angle.");
        }
    }
}
```

### Voir aussi

* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


