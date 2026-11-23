---
title: "Shape.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le nom de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/name/
---
## Shape.Name property

Obtient et définit le nom de la forme.

```csharp
public string Name { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez une forme et définissez son nom
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Name = "shape1";
            
            // Vérifiez que le nom a été défini
            Console.WriteLine("Shape name: " + shape.Name);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


