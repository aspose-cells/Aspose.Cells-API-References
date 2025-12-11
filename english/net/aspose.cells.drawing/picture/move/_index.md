---
title: Picture.Move
second_title: Aspose.Cells for .NET API Reference
description: Picture method. Moves the picture to a specified location
type: docs
url: /net/aspose.cells.drawing/picture/move/
---
## Picture.Move method

Moves the picture to a specified location.

```csharp
public void Move(int topRow, int leftColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |

### Examples

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

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


