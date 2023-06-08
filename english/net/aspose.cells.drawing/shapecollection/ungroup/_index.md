---
title: ShapeCollection.Ungroup
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Ungroups the shape items
type: docs
url: /net/aspose.cells.drawing/shapecollection/ungroup/
---
## ShapeCollection.Ungroup method

Ungroups the shape items.

```csharp
public void Ungroup(GroupShape group)
```

| Parameter | Type | Description |
| --- | --- | --- |
| group | GroupShape | The group shape. |

### Remarks

If the group shape is grouped by another group shape,nothing will be done.

### Examples

```csharp

[C#]
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//group
Shape[] shapesArr = new Shape[] { shapes[0], shapes[1] };
GroupShape groupShape = shapes.Group(shapesArr);

//ungroup
shapes.Ungroup(groupShape);

```

### See Also

* class [GroupShape](../../groupshape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


