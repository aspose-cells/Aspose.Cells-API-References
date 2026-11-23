---
title: "Shape.ActualLowerRightRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtenez la ligne inférieure réelle"
type: docs
url: /fr/net/aspose.cells.drawing/shape/actuallowerrightrow/
---
## Shape.ActualLowerRightRow property

Obtenir la ligne inférieure réelle.

```csharp
public int ActualLowerRightRow { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyActualLowerRightRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme d'exemple (rectangle)
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 100);

            // Obtenez la ligne inférieure droite réelle de la forme
            int actualLowerRightRow = shape.ActualLowerRightRow;

            // Afficher le résultat
            Console.WriteLine("Actual Lower Right Row of the shape: " + actualLowerRightRow);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


