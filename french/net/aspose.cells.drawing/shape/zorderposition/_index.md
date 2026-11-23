---
title: "Shape.ZOrderPosition"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Retourne la position d'une forme dans l'ordre Z"
type: docs
url: /fr/net/aspose.cells.drawing/shape/zorderposition/
---
## Shape.ZOrderPosition property

Renvoie la position d'une forme dans l'ordre Z.

```csharp
public int ZOrderPosition { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyZOrderPositionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter trois formes pour démontrer ZOrder
            Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);
            Shape shape3 = worksheet.Shapes.AddRectangle(90, 90, 100, 100, 0, 0);

            // Définir les positions ZOrder
            shape1.ZOrderPosition = 0;
            shape2.ZOrderPosition = 1;
            shape3.ZOrderPosition = 2;

            // Changer le ZOrder de shape3 pour le mettre au premier plan
            shape3.ZOrderPosition = 0;

            // Enregistrez le classeur
            workbook.Save("ShapeZOrderDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


