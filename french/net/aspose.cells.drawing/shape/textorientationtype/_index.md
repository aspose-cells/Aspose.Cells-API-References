---
title: "Shape.TextOrientationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le type d'orientation du texte de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/textorientationtype/
---
## Shape.TextOrientationType property

Obtient et définit le type d'orientation du texte de la forme.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);

            // Définir le texte pour la forme
            shape.Text = "Sample Text";

            // Vérifier et modifier l'orientation du texte
            if (shape.TextOrientationType == TextOrientationType.NoRotation)
            {
                shape.TextOrientationType = TextOrientationType.TopToBottom;
            }

            // Enregistrez le classeur
            workbook.Save("ShapeTextOrientationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextOrientationType](../../../aspose.cells/textorientationtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


