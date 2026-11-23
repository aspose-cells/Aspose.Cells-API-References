---
title: "Shape.IsAspectRatioLocked"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. True signifie que le ratio d'aspect de la forme est verrouillé"
type: docs
url: /fr/net/aspose.cells.drawing/shape/isaspectratiolocked/
---
## Shape.IsAspectRatioLocked property

Vrai signifie que le rapport d'aspect de la forme est verrouillé.

```csharp
public bool IsAspectRatioLocked { get; set; }
```

### Remarques

Uniquement pour les images et les objets Ole.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsAspectRatioLockedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 50);
            
            Console.WriteLine("Original Aspect Ratio Locked: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = true;
            Console.WriteLine("After setting to true: " + shape.IsAspectRatioLocked);
            
            shape.IsAspectRatioLocked = false;
            Console.WriteLine("After setting to false: " + shape.IsAspectRatioLocked);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


