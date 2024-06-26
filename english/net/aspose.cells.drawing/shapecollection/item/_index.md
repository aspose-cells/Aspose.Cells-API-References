---
title: ShapeCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection property. Gets the Shape object at the specific index in the list
type: docs
url: /net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Gets the [`Shape`](../../shape/) object at the specific index in the list.

```csharp
public Shape this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp

[C#]
//get the first shape
Shape shape = shapes[0];
```

### See Also

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Gets the [`Shape`](../../shape/) object by the name of the shape.

```csharp
public Shape this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the shape. |

### Examples

```csharp

[C#]
//add a shape
shapes.AddRectangle(2, 0, 2, 0, 130, 130);
//get the shape by the name.
Shape shape1 = shapes["Rectangle 1"];
if(shape1 != null)
{
    //Got the shape named 'Rectangle 1'.
}
```

### See Also

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


