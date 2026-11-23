---
title: "Shape.MsoDrawingType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient le type de dessin"
type: docs
url: /fr/net/aspose.cells.drawing/shape/msodrawingtype/
---
## Shape.MsoDrawingType property

Obtient le type de dessin.

```csharp
public MsoDrawingType MsoDrawingType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMsoDrawingTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangle (paramètres corrigés)
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            
            // Obtenez et affichez le MsoDrawingType de la forme
            MsoDrawingType drawingType = rectangle.MsoDrawingType;
            Console.WriteLine("Shape MsoDrawingType: " + drawingType.ToString());

            // Ajoutez une forme ligne (paramètres corrigés)
            Shape line = worksheet.Shapes.AddLine(3, 0, 3, 100, 150, 1);
            
            // Obtenez et affichez le MsoDrawingType de la ligne
            drawingType = line.MsoDrawingType;
            Console.WriteLine("Line MsoDrawingType: " + drawingType.ToString());
        }
    }
}
```

### Voir aussi

* enum [MsoDrawingType](../../msodrawingtype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


