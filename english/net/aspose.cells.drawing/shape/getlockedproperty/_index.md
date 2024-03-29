---
title: Shape.GetLockedProperty
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Gets the value of locked property
type: docs
url: /net/aspose.cells.drawing/shape/getlockedproperty/
---
## Shape.GetLockedProperty method

Gets the value of locked property.

```csharp
public bool GetLockedProperty(ShapeLockType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ShapeLockType | The type of the shape locked property. |

### Return Value

Returns the value of locked property.

### Examples

```csharp

[C#]
int noAdjustHandles = 0;
if (shape.GetLockedProperty(ShapeLockType.AdjustHandles))
    noAdjustHandles = 1;
```

### See Also

* enum [ShapeLockType](../../shapelocktype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


