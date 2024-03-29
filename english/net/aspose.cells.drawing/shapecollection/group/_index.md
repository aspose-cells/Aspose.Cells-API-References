---
title: ShapeCollection.Group
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Group the shapes
type: docs
url: /net/aspose.cells.drawing/shapecollection/group/
---
## ShapeCollection.Group method

Group the shapes.

```csharp
public GroupShape Group(Shape[] groupItems)
```

| Parameter | Type | Description |
| --- | --- | --- |
| groupItems | Shape[] | the group items. |

### Return Value

Return the group shape.

### Remarks

The shape in the groupItems should not be grouped. The shape must be in this Shapes collection.

### Examples

```csharp

[C#]
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };
GroupShape groupShape = shapes.Group(shapesArr);

```

### See Also

* class [GroupShape](../../groupshape/)
* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


