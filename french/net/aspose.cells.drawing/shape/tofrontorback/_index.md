---
title: "Shape.ToFrontOrBack"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Shape. Amène la forme à l'avant ou l'envoie à l'arrière"
type: docs
url: /fr/net/aspose.cells.drawing/shape/tofrontorback/
---
## Shape.ToFrontOrBack method

Place la forme au premier plan ou envoie la forme à l'arrière-plan.

```csharp
public void ToFrontOrBack(int orders)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ordres | Int32 | Si c'est inférieur à zéro, place la forme à l'arrière. Si c'est supérieur à zéro, amène la forme à l'avant. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodToFrontOrBackWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez deux formes pour démontrer l'ordre Z
            Aspose.Cells.Drawing.Shape shape1 = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);
            Aspose.Cells.Drawing.Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Déplacez shape2 de 2 positions vers l'avant dans l'ordre Z
            shape2.ToFrontOrBack(2);

            // Déplacez shape1 de 1 position vers l'arrière dans l'ordre Z
            shape1.ToFrontOrBack(-1);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


