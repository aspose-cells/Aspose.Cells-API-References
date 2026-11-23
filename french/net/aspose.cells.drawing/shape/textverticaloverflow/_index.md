---
title: "Shape.TextVerticalOverflow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le type de dépassement vertical du texte de la forme qui contient du texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/textverticaloverflow/
---
## Shape.TextVerticalOverflow property

Obtient et définit le type de dépassement vertical du texte de la forme qui contient du texte.

```csharp
public TextOverflowType TextVerticalOverflow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextVerticalOverflowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
            
            // Définir le texte et le faire dépasser verticalement
            shape.Text = "This is a long text that will demonstrate vertical text overflow functionality in the shape.";
            shape.TextVerticalOverflow = TextOverflowType.Overflow;

            // Enregistrez le classeur
            workbook.Save("ShapeTextVerticalOverflowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextOverflowType](../../textoverflowtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


