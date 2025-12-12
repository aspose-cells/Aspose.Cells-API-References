---
title: ShapeCollection.AddAutoShape
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a AutoShape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addautoshape/
---
## ShapeCollection.AddAutoShape method

Adds a AutoShape to the worksheet.

```csharp
public Shape AddAutoShape(AutoShapeType type, int topRow, int top, int leftColumn, int left, 
    int height, int width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | AutoShapeType | Auto shape type. |
| topRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Shape from its left row, in unit of pixel. |
| leftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Shape, in unit of pixel. |
| width | Int32 | Represents the width of Shape, in unit of pixel. |

### Return Value

A Shape object.

### Remarks

The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddAutoShapeWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            ShapeCollection shapes = worksheet.Shapes;
            Shape autoShape = shapes.AddAutoShape(AutoShapeType.Cube, 1, 0, 1, 0, 100, 50);
            
            workbook.Save("AutoShapeDemo.xlsx");
        }
    }
}
```

### See Also

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


