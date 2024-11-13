---
title: ShapeCollection.AddFreeform
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a freeform shape to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

Adds a freeform shape to the worksheet.

```csharp
public Shape AddFreeform(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width, ShapePath[] paths)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| top | Int32 | Represents the vertical offset of Polygon from its left row, in unit of pixel. |
| upperLeftColumn | Int32 | Upper left column index. |
| left | Int32 | Represents the horizontal offset of Polygon from its left column, in unit of pixel. |
| height | Int32 | Represents the height of Polygon, in unit of pixel. |
| width | Int32 | Represents the width of Polygon, in unit of pixel. |
| paths | ShapePath[] | Represents a user-defined path |

### Return Value

A freeform shape.

### Examples

```csharp

[C#]
//Custom figure
ShapePath shapePath = new ShapePath();
shapePath.MoveTo(60, 45);
shapePath.ArcTo(25, 25, 0, 270);
shapePath.Close();

shapePath.MoveTo(60, 20);
shapePath.LineTo(110, 70);
shapePath.LineTo(125, 155.5f);
shapePath.ArcTo(35.5f, 35.5f, 0, 270);
shapePath.Close();

shapePath.MoveTo(150, 45);
shapePath.ArcTo(25, 25, 0, 270);

ShapePath shapePath1 = new ShapePath();
shapePath1.MoveTo(0, 0);
shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                    96.5f, -7.148871f,
                    130, 11.517795f);
shapePath1.CubicBezierTo(163.5f, 30.18446f,
                    182.24997f, 75.351f,
                    201, 120.517795f);
shapePath1.MoveTo(150, 80);
shapePath1.ArcTo(25, 25, 0, 270);

//Insert custom figure into worksheet
shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1});

```

### See Also

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


