---
title: "ThreeDFormat.TopBevelType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ThreeDFormat. Obtient et définit le type du biseau supérieur ou la profondeur d'application dans la forme. En unités de points"
type: docs
url: /fr/net/aspose.cells.drawing/threedformat/topbeveltype/
---
## ThreeDFormat.TopBevelType property

Obtient et définit le type du biseau supérieur, ou la profondeur d'application dans la forme. En unité de points.

```csharp
public BevelType TopBevelType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            workbook.Save("ThreeDFormatTopBevelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


