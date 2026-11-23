---
title: "ThreeDFormat.TopBevelHeight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit la hauteur du chanfrein supérieur ou la profondeur d'application dans la forme. En unité de points"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/topbevelheight/
---
## ThreeDFormat.TopBevelHeight property

Obtient et définit la hauteur du biseau supérieur, ou la profondeur d'application dans la forme. En unités de points.

```csharp
public double TopBevelHeight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.Circle;
            threeDFormat.TopBevelHeight = 15;
            threeDFormat.TopBevelWidth = 10;

            workbook.Save("ThreeDFormatTopBevelHeightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


