---
title: Aspose::Cells::Drawing::ShapeCollection::AddFreeform method
linktitle: AddFreeform
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddFreeform method. Adds a freeform shape to the worksheet in C++.'
type: docs
weight: 5200
url: /cpp/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection::AddFreeform method


Adds a freeform shape to the worksheet.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddFreeform(int32_t upperLeftRow, int32_t top, int32_t upperLeftColumn, int32_t left, int32_t height, int32_t width, const Vector<ShapePath> &paths)
```


| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of Polygon from its left row, in unit of pixel. |
| upperLeftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of Polygon from its left column, in unit of pixel. |
| height | int32_t | Represents the height of Polygon, in unit of pixel. |
| width | int32_t | Represents the width of Polygon, in unit of pixel. |
| paths | const Vector \<ShapePath\>\& | Represents a user-defined path |

## ReturnValue

A freeform shape.


## Examples


```cpp
    //Custom figure
ShapePath shapePath;
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

ShapePath shapePath1;
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
shapes.AddFreeform(1, 0, 1, 0, 200, 200, Vector<ShapePath>{ shapePath, shapePath1 });
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapePath](../../shapepath/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
