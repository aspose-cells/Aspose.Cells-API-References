---
title: "GradientFill.FillType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété GradientFill. Obtient le type de remplissage du dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Obtient le type de remplissage en dégradé.

```csharp
public GradientFillType FillType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme avec un remplissage dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Définir les propriétés du dégradé
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Afficher le type de remplissage du dégradé
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Passer à un dégradé radial
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Enregistrez le classeur
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


