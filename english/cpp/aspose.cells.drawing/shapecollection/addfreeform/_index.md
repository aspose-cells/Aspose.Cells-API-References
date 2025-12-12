---
title: Aspose::Cells::Drawing::ShapeCollection::AddFreeform method
linktitle: AddFreeform
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddFreeform method. Adds a freeform shape to the worksheet in C++.'
type: docs
weight: 5300
url: /cpp/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection::AddFreeform method


Adds a freeform shape to the worksheet.

```cpp
Shape Aspose::Cells::Drawing::ShapeCollection::AddFreeform(int32_t topRow, int32_t top, int32_t leftColumn, int32_t left, int32_t height, int32_t width, const Vector<ShapePath> &paths)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| top | int32_t | Represents the vertical offset of freeform shape from its left row, in unit of pixel. |
| leftColumn | int32_t | Upper left column index. |
| left | int32_t | Represents the horizontal offset of freeform shape from its left column, in unit of pixel. |
| height | int32_t | Represents the height of freeform shape, in unit of pixel. |
| width | int32_t | Represents the width of freeform shape, in unit of pixel. |
| paths | const Vector \<ShapePath\>\& | Represents a user-defined path |

## ReturnValue

A freeform shape.
## Remarks



Notice: That the width and height in the parameters can be any positive integer values, not the total width and height of the [ShapePath](../../shapepath/) array specified by ’paths'. The relationship between them is a scale-fill relationship, that is, each [ShapePath](../../shapepath/) object will be scaled according to the width and height. Therefore, when there are multiple objects in the 'paths', each [ShapePath](../../shapepath/) object needs to be designed reasonably to meet expectations. When there is only one [ShapePath](../../shapepath/) object and there are no other requirements, passing the object's width and height as parameter values ​​is a good solution.

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

int shapePathW = shapePath.GetWidthPixel();
int shapePathH = shapePath.GetHeightPixel();

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

if (shapePath1.GetWidthPixel() > shapePathW)
{
    shapePathW = shapePath1.GetWidthPixel();
}

if (shapePath1.GetHeightPixel() > shapePathH)
{
    shapePathH = shapePath1.GetHeightPixel();
}

//Notice: shapePathH and shapePathH can be any positive integer values, here we just simply set them.

//Insert custom figure into worksheet
shapes.AddFreeform(1, 0, 1, 0, shapePathH, shapePathW, Vector<ShapePath>{ shapePath, shapePath1 });
```

## See Also

* Class [Shape](../../shape/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [ShapePath](../../shapepath/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
