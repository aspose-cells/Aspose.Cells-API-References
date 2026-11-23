---
title: "Shape.IsHidden"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si l'objet est visible"
type: docs
url: /fr/net/aspose.cells.drawing/shape/ishidden/
---
## Shape.IsHidden property

Indique si l'objet est visible.

```csharp
public bool IsHidden { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme à la feuille de calcul
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Définissez la propriété IsHidden sur false (visible)
            shape.IsHidden = false;
            Console.WriteLine("Shape is visible: " + !shape.IsHidden);

            // Définissez la propriété IsHidden sur true (caché)
            shape.IsHidden = true;
            Console.WriteLine("Shape is hidden: " + shape.IsHidden);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


