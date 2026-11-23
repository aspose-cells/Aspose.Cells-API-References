---
title: "Shape.IsTextWrapped"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le type d'habillage du texte de la forme qui contient du texte"
type: docs
url: /fr/net/aspose.cells.drawing/shape/istextwrapped/
---
## Shape.IsTextWrapped property

Obtient et définit le type d'habillage du texte de la forme qui contient du texte.

```csharp
public bool IsTextWrapped { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsTextWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme et définissez du texte
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);
            shape.Text = "This is a sample text that will demonstrate text wrapping functionality";

            // Démontrer la propriété IsTextWrapped
            Console.WriteLine("Initial IsTextWrapped value: " + shape.IsTextWrapped);
            
            // Basculer l'habillage du texte
            shape.IsTextWrapped = !shape.IsTextWrapped;
            Console.WriteLine("After toggle, IsTextWrapped value: " + shape.IsTextWrapped);

            // Enregistrez le classeur
            workbook.Save("ShapeTextWrappingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


