---
title: "Picture.Move"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Picture-metod. Flyttar bilden till en angiven plats"
type: docs
url: /sv/net/aspose.cells.drawing/picture/move/
---
## Picture.Move method

Flyttar bilden till en angiven plats.

```csharp
public void Move(int topRow, int leftColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.Move(2, 4);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Se även

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


