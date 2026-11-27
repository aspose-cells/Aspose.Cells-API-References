---
title: "ShapeCollection.AddActiveXControl"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Skapar en Activex-kontroll"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addactivexcontrol/
---
## ShapeCollection.AddActiveXControl method

Skapar en Activex-kontroll.

```csharp
public Shape AddActiveXControl(ControlType type, int topRow, int top, int leftColumn, int left, 
    int width, int height)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ControlType | Kontrollens typ. |
| topRow | Int32 | Övre vänstra radindex. |
| top | Int32 | Representerar den vertikala förskjutningen av Shape från dess vänstra rad, i enheten pixel. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| vänster | Int32 | Representerar den horisontella förskjutningen av Shape från dess vänstra kolumn, i enheten pixel. |
| höjd | Int32 | Representerar höjden på Shape, i enheten pixel. |
| bredd | Int32 | Representerar bredden på Shape, i enheten pixel. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddActiveXControlWithControlTypeInt32Int32Int32Int3Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape activeXControl = shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 
                1,  // upperLeftRow
                0,  // top
                1,  // upperLeftColumn
                0,  // left
                100,  // width
                50   // height
            );

            workbook.Save("AddActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [ControlType](../../../aspose.cells.drawing.activexcontrols/controltype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


