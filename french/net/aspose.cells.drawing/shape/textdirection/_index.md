---
title: "Shape.TextDirection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient/Définit la direction du flux de texte pour cet objet"
type: docs
url: /fr/net/aspose.cells.drawing/shape/textdirection/
---
## Shape.TextDirection property

Obtient/Définit la direction du flux de texte pour cet objet.

```csharp
public TextDirectionType TextDirection { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextDirectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de texte
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample Text";

            // Définir et démontrer la propriété TextDirection
            shape.TextDirection = TextDirectionType.Context;
            Console.WriteLine("Initial TextDirection: " + shape.TextDirection);

            // Changer la direction du texte
            shape.TextDirection = TextDirectionType.LeftToRight;
            Console.WriteLine("Updated TextDirection: " + shape.TextDirection);

            // Enregistrez le classeur
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


