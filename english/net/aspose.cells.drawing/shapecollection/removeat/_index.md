---
title: ShapeCollection.RemoveAt
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Remove the shape
type: docs
url: /net/aspose.cells.drawing/shapecollection/removeat/
---
## ShapeCollection.RemoveAt method

Remove the shape.

```csharp
public void RemoveAt(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the shape. |

### Examples

```csharp

[C#]
//add first shape
shapes.AddRectangle(2, 0, 2, 0, 50, 50);
//add second shape
shapes.AddRectangle(6, 0, 2, 0, 30, 30);

//remove 
shapes.RemoveAt(0);

```

### See Also

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


