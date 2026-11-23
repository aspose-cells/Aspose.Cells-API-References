---
title: "Shape.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient le type de forme automatique"
type: docs
url: /fr/net/aspose.cells.drawing/shape/type/
---
## Shape.Type property

Obtient le type de forme auto.

```csharp
public AutoShapeType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un shape rectangle avec les paramètres corrects
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Obtenir et afficher le type de forme
            AutoShapeType autoShapeType = shape.Type;
            Console.WriteLine("Shape Type: " + autoShapeType);

            // Impossible de changer le type de forme car la propriété Type est en lecture seule
            // Créez plutôt une nouvelle forme avec un type différent
            Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
            Console.WriteLine("New Shape Type: " + ovalShape.Type);
        }
    }
}
```

### Voir aussi

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


