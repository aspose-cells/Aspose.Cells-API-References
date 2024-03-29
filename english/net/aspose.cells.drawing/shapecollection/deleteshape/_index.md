---
title: ShapeCollection.DeleteShape
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Delete a shape. If the shape is in the group or is a comment shape it will not be deleted
type: docs
url: /net/aspose.cells.drawing/shapecollection/deleteshape/
---
## ShapeCollection.DeleteShape method

Delete a shape. If the shape is in the group or is a comment shape, it will not be deleted.

```csharp
public void DeleteShape(Shape shape)
```

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape |  |

### Examples

```csharp

[C#]
//add first shape
Shape firstShape = shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
Shape secondShape = shapes.AddRectangle(6, 0, 2, 0, 30, 30);
//del
shapes.DeleteShape(firstShape);

```

### See Also

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


