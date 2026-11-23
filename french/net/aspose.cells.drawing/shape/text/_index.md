---
title: "Shape.Text"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le texte de cette forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/text/
---
## Shape.Text property

Obtient et définit le texte de cette forme.

```csharp
public string Text { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Définissez le texte si null
            if (shape.Text == null)
            {
                shape.Text = "This is a test.";
            }

            // Modifiez le texte
            shape.Text = "Updated text demo";

            // Enregistrez le classeur
            workbook.Save("ShapeTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


