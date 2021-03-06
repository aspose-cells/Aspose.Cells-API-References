---
title: GetLockedProperty
second_title: Aspose.Cells for .NET API Reference
description: Gets the value of locked property.
type: docs
weight: 1110
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

* enum [ShapeLockType](../../shapelocktype)
* class [Shape](../../shape)
* namespace [Aspose.Cells.Drawing](../../shape)
* assembly [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
