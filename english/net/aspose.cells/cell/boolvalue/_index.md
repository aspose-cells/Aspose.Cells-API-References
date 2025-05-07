---
title: Cell.BoolValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the boolean value contained in the cell
type: docs
url: /net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Gets the boolean value contained in the cell.

```csharp
public bool BoolValue { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(false, cells[0, 255].BoolValue, "cells[0, 255].BoolValue");
private void Property_BoolValue(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            AssertHelper.AreEqual(1, cells[0, 0].IntValue, "cells[0, 0].IntValue");
            AssertHelper.AreEqual(2.1, cells[0, 1].DoubleValue, "cells[0, 1].DoubleValue");
            AssertHelper.AreEqual(null, cells[0, 2].Value, "cells[0, 2].Value");
            AssertHelper.AreEqual(true, cells[0, 3].BoolValue, "cells[0, 3].BoolValue");
            AssertHelper.AreEqual("abc", cells[0, 4].StringValue, "cells[0, 4].StringValue");
            AssertHelper.AreEqual(false, cells[0, 255].BoolValue, "cells[0, 255].BoolValue");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


