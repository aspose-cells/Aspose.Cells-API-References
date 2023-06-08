---
title: Shape.GetInputRange
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Gets the range used to fill the control
type: docs
url: /net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Gets the range used to fill the control.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Return Value

The range used to fill the control.

### Examples

```csharp

[C#]
string range = shape.GetInputRange(false, true);
//If successful, a value like "$A$1:$A$3" will be returned
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


