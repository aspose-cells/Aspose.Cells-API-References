---
title: "ThreeDFormat.BottomBevelHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la hauteur du chanfrein inférieur ou la profondeur d'application dans la forme. En unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/bottombevelheight/
---
## ThreeDFormat.BottomBevelHeight property

Obtient et définit la hauteur du biseau inférieur, ou la profondeur d'application dans la forme. En unités de points.

```csharp
public double BottomBevelHeight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.BottomBevelType = BevelType.Circle;
            threeDFormat.BottomBevelWidth = 8;
            threeDFormat.BottomBevelHeight = 12;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


