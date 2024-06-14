---
title: Shape.IsLocked
second_title: Aspose.Cells for .NET API Reference
description: Shape property. True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected
type: docs
url: /net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```csharp
public bool IsLocked { get; set; }
```

### Examples

```csharp

[C#]
//Sets the specified shape to unlocked state
if (shape.Worksheet.IsProtected && shape.IsLocked)
{
    shape.IsLocked = false;
}

//Sets the specified shape to a locked state
if (shape.Worksheet.IsProtected && !shape.IsLocked)
{
    shape.IsLocked = true;
}

```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


