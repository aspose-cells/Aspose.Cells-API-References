---
title: "ShapeCollection.AddOleObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till ett OleObject"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addoleobject/
---
## ShapeCollection.AddOleObject method

Lägger till ett OleObject.

```csharp
public OleObject AddOleObject(int topRow, int top, int leftColumn, int left, int height, int width, 
    byte[] imageData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 |  |
| top | Int32 |  |
| leftColumn | Int32 |  |
| vänster | Int32 |  |
| höjd | Int32 |  |
| bredd | Int32 |  |
| imageData | Byte[] |  |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddOleObjectWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            byte[] imageData = File.ReadAllBytes("image.jpg");
            shapes.AddOleObject(4, 0, 5, 0, 300, 500, imageData);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [OleObject](../../oleobject/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


