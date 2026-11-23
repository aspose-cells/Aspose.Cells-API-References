---
title: "GradientFill.DirectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientFill. Obtient le type de direction du dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/directiontype/
---
## GradientFill.DirectionType property

Obtient le type de direction du dégradé.

```csharp
public GradientDirectionType DirectionType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyDirectionTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour démontrer le remplissage dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 5);

            // Définir les propriétés de remplissage de dégradé
            FillFormat fillFormat = shape.Fill;
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.DiagonalDown, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Afficher le type de direction du gradient
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Enregistrez le classeur
            workbook.Save("GradientDirectionTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


