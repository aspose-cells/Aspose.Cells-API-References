---
title: "Shape.AnchorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient et définit le type du placeholder d'ancrage de forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/anchortype/
---
## Shape.AnchorType property

Obtient et définit le type de l'espace réservé d'ancrage de forme.

```csharp
public ShapeAnchorType AnchorType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme avec le type d'ancrage par défaut
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            
            // Vérifiez et modifiez le type d'ancrage
            if (shape.AnchorType == ShapeAnchorType.OneCellAnchor)
            {
                shape.AnchorType = ShapeAnchorType.TwoCellAnchor;
                Console.WriteLine("Anchor type changed to TwoCellAnchor");
            }
            
            // Enregistrez le classeur
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ShapeAnchorType](../../shapeanchortype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


