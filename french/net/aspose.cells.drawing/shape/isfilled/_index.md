---
title: "Shape.IsFilled"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Indique si le format de remplissage est visible"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isfilled/
---
## Shape.IsFilled property

Indique si le format de remplissage est visible.

```csharp
public bool IsFilled { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsFilledDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 150, 200);

            // Vérifier et modifier la propriété IsFilled
            if (shape.IsFilled == false)
            {
                shape.IsFilled = true;
                shape.FillFormat.ForeColor = System.Drawing.Color.Red;
            }

            // Enregistrez le classeur
            workbook.Save("ShapeIsFilledDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


