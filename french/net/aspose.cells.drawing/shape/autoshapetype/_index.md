---
title: "Shape.AutoShapeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le type de forme automatique"
type: docs
url: /fr/net/aspose.cells.drawing/shape/autoshapetype/
---
## Shape.AutoShapeType property

Obtient et définit le type de forme automatique.

```csharp
public AutoShapeType AutoShapeType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAutoShapeTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme à la feuille de calcul avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Vérifiez et modifiez le AutoShapeType si nécessaire
            if (shape.AutoShapeType == AutoShapeType.Unknown)
            {
                shape.AutoShapeType = AutoShapeType.Rectangle;
            }

            // Modifiez le type de forme pour démontrer la propriété
            shape.AutoShapeType = AutoShapeType.Oval;

            // Enregistrez le classeur
            workbook.Save("ShapePropertyAutoShapeTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


