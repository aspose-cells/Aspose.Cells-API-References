---
title: Cell.Value
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets/sets the value contained in this cell
type: docs
url: /net/aspose.cells/cell/value/
---
## Cell.Value property

Gets/sets the value contained in this cell.

```csharp
public object Value { get; set; }
```

### Remarks

Possible type:

null,

Boolean,

DateTime,

Double,

Integer

String.

For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

### Examples

```csharp
// Called: AssertHelper.AreEqual(null, cells[6, 4].Value, "cells[6, 4].Value");
private void Property_Value(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            AssertHelper.AreEqual(null, cells[2, 0].Value, "cells[2, 0].Value");
            AssertHelper.AreEqual("=SUM(B4:D4)", cells[3, 0].Formula, "cells[3, 0].Formula");
            AssertHelper.AreEqual("=SUM(B5:D5)", cells[4, 0].Formula, "cells[4, 0].Formula");
            AssertHelper.AreEqual("=SUM(B6:D6)", cells[5, 0].Formula, "cells[5, 0].Formula");
            AssertHelper.AreEqual(null, cells[6, 0].Value, "cells[6, 0].Value");
            AssertHelper.AreEqual("=SUM(B4:B6)", cells[2, 1].Formula, "cells[2, 1].Formula");
            AssertHelper.AreEqual(1, cells[3, 1].IntValue, "cells[3, 1].IntValue");
            AssertHelper.AreEqual(2, cells[4, 1].IntValue, "cells[4, 1].IntValue");
            AssertHelper.AreEqual(3, cells[5, 1].IntValue, "cells[5, 1].IntValue");
            AssertHelper.AreEqual("=SUM(B4:B6)", cells[6, 1].Formula, "cells[6, 1].Formula");
            AssertHelper.AreEqual("=SUM(C4:C6)", cells[2, 2].Formula, "cells[2, 2].Formula");
            AssertHelper.AreEqual(4, cells[3, 2].IntValue, "cells[3, 2].IntValue");
            AssertHelper.AreEqual(5, cells[4, 2].IntValue, "cells[4, 2].IntValue");
            AssertHelper.AreEqual(6, cells[5, 2].IntValue, "cells[5, 2].IntValue");
            AssertHelper.AreEqual("=SUM(C4:C6)", cells[6, 2].Formula, "cells[6, 2].Formula");
            AssertHelper.AreEqual("=SUM(D4:D6)", cells[2, 3].Formula, "cells[2, 3].Formula");
            AssertHelper.AreEqual(7, cells[3, 3].IntValue, "cells[3, 3].IntValue");
            AssertHelper.AreEqual(8, cells[4, 3].IntValue, "cells[4, 3].IntValue");
            AssertHelper.AreEqual(9, cells[5, 3].IntValue, "cells[5, 3].IntValue");
            AssertHelper.AreEqual("=SUM(D4:D6)", cells[6, 3].Formula, "cells[6, 3].Formula");
            AssertHelper.AreEqual(null, cells[2, 4].Value, "cells[2, 4].Value");
            AssertHelper.AreEqual("=SUM(B4:D4)", cells[3, 4].Formula, "cells[3, 4].Formula");
            AssertHelper.AreEqual("=SUM(B5:D5)", cells[4, 4].Formula, "cells[4, 4].Formula");
            AssertHelper.AreEqual("=SUM(B6:D6)", cells[5, 4].Formula, "cells[5, 4].Formula");
            AssertHelper.AreEqual(null, cells[6, 4].Value, "cells[6, 4].Value");
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


