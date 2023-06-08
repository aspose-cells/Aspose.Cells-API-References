---
title: ShapeCollection.Remove
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Remove the shape
type: docs
url: /net/aspose.cells.drawing/shapecollection/remove/
---
## ShapeCollection.Remove method

Remove the shape.

```csharp
public void Remove(Shape shape)
```

| Parameter | Type | Description |
| --- | --- | --- |
| shape | Shape |  |

### Examples

```csharp

[C#]
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//get the shape
Shape s = shapes["Rectangle 1"];// or shapes[0];
if (s != null)
{
    //remove 
    shapes.Remove(s);
}
```

### See Also

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


