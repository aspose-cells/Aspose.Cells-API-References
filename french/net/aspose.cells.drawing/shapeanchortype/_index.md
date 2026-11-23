---
title: "Enum ShapeAnchorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ShapeAnchorType enum. Représente le type d'ancrage"
type: docs
url: /fr/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

Représente le type d'ancre.

```csharp
public enum ShapeAnchorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| TwoCellAnchor | `0` | Représente un espace réservé d'ancrage à deux cellules |
| OneCellAnchor | `1` | Représente un espace réservé d'ancrage à une cellule |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de zone de groupe
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // Démontrer l'utilisation de ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // Enregistrez le classeur
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


