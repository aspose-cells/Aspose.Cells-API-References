---
title: "Enum GradientFillType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.GradientFillType enum. Représente tous les types de remplissage dégradé"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfilltype/
---
## GradientFillType enumeration

Représente tous les types de remplissage de dégradé.

```csharp
public enum GradientFillType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Linear | `0` | Linéaire |
| Radial | `1` | Radial |
| Rectangle | `2` | Rectangle |
| Path | `3` | Chemin |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassGradientFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une forme pour démontrer le remplissage dégradé
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 5, 20);

            // Obtenir le format de remplissage
            FillFormat fillFormat = shape.Fill;

            // Définir le type de remplissage dégradé et ses propriétés
            fillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.LightBlue, GradientStyleType.Horizontal, 1);
            fillFormat.GradientFill.SetGradient(GradientFillType.Linear, 45, GradientDirectionType.FromUpperLeftCorner);

            // Afficher le type de direction du dégradé
            Console.WriteLine("Gradient Direction Type: " + fillFormat.GradientFill.DirectionType);

            // Enregistrez le classeur
            workbook.Save("GradientFillTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


