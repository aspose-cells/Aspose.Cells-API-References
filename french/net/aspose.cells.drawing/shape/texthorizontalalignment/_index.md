---
title: "Shape.TextHorizontalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Shape property. Obtient et définit le type d'alignement horizontal du texte du shape"
type: docs
url: /fr/net/aspose.cells.drawing/shape/texthorizontalalignment/
---
## Shape.TextHorizontalAlignment property

Obtient et définit le type d'alignement horizontal du texte de la forme.

```csharp
public TextAlignmentType TextHorizontalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextHorizontalAlignmentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Définir le texte et l'alignement
            shape.Text = "Sample Text";
            shape.TextHorizontalAlignment = TextAlignmentType.Center;

            // Modifier l'alignement s'il est actuellement Bottom
            if (shape.TextHorizontalAlignment == TextAlignmentType.Bottom)
            {
                shape.TextHorizontalAlignment = TextAlignmentType.Center;
            }

            // Enregistrez le classeur
            workbook.Save("ShapeTextAlignmentDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


