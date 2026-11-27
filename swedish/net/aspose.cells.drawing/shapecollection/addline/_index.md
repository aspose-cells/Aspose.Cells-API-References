---
title: "ShapeCollection.AddLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en LineShape till kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addline/
---
## ShapeCollection.AddLine method

Lägger till en LineShape i kalkylbladet.

```csharp
public LineShape AddLine(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för LineShape från dess vänstra rad, i enheten pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella offsetet för LineShape från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar höjden på LineShape, i enheten pixel. |
| bredd | Int32 | Representerar bredden på LineShape, i enheten pixel. |

### Returvärde

Ett LineShape-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddLineWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            LineShape lineShape = shapes.AddLine(1, 0, 1, 0, 100, 50);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [LineShape](../../lineshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


