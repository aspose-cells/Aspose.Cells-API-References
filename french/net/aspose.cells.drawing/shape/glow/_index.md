---
title: "Shape.Glow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente un objet GlowEffect qui spécifie l'effet de lueur pour l'élément de graphique ou la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/glow/
---
## Shape.Glow property

Représente un objet [`GlowEffect`](../../gloweffect/) qui spécifie l'effet de lueur pour l'élément de graphique ou la forme.

```csharp
public GlowEffect Glow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGlowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);

            // Accéder à l'effet de lueur
            GlowEffect glow = shape.Glow;

            // Définir les propriétés de la lueur
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Purple;
            glow.Color = color;
            glow.Size = 10; // 10 point radius
            glow.Transparency = 0.5; // 50% transparency

            // Enregistrez le classeur
            workbook.Save("ShapeGlowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GlowEffect](../../gloweffect/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


