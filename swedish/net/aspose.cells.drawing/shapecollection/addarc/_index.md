---
title: "ShapeCollection.AddArc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en ArcShape till kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addarc/
---
## ShapeCollection.AddArc method

Lägger till en ArcShape i kalkylbladet.

```csharp
public ArcShape AddArc(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar det vertikala offsetet för ArcShape från dess vänstra rad, i enheten pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar det horisontella offsetet för ArcShape från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar höjden på ArcShape, i enheten pixel. |
| bredd | Int32 | Representerar bredden på ArcShape, i enheten pixel. |

### Returvärde

Ett ArcShape-objekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddArcWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            ArcShape arcShape = shapes.AddArc(10, 10, 100, 50, 45, 180);
            
            workbook.Save("AddArcDemo.xlsx");
        }
    }
}
```

### Se även

* class [ArcShape](../../arcshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


