---
title: "Shape.Line"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient le style de ligne"
type: docs
url: /fr/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

Obtient le style de ligne

```csharp
public LineFormat Line { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme de ligne (renvoie directement LineShape)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // Accéder et modifier les propriétés de la ligne
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Enregistrez le classeur
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


