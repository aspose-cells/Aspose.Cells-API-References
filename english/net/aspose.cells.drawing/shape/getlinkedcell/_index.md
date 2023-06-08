---
title: Shape.GetLinkedCell
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Gets the range linked to the controls value
type: docs
url: /net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Gets the range linked to the control's value.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |

### Return Value

The range linked to the control's value.

### Examples

```csharp

[C#]
//You may get results like '$A$1'
string link = shape.GetLinkedCell(false, false);
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


