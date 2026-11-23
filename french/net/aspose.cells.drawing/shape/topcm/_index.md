---
title: "Shape.TopCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Représente le décalage vertical de la forme depuis sa ligne supérieure, en centimètres."
type: docs
url: /fr/net/aspose.cells.drawing/shape/topcm/
---
## Shape.TopCM property

Représente le décalage vertical de la forme par rapport à sa ligne supérieure, en centimètres.

```csharp
public double TopCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape.TopCM = 3.0;
            
            Console.WriteLine("Shape Top position (cm): " + shape.TopCM);
            
            if (shape.TopCM == 3.0)
                shape.TopCM = 1.0;
                
            Console.WriteLine("Shape Top position after change (cm): " + shape.TopCM);
        }
    }
}
```

### Voir aussi

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


