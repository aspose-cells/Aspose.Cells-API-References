---
title: Cell.IsNumericValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether the value of this cell is numericint double and datetime
type: docs
url: /net/aspose.cells/cell/isnumericvalue/
---
## Cell.IsNumericValue property

Indicates whether the value of this cell is numeric(int, double and datetime)

```csharp
public bool IsNumericValue { get; }
```

### Remarks

Also applies to formula cell to check the calculated result

### Examples

```csharp
// Called: if (!c.IsNumericValue)
public static void Cell_Property_IsNumericValue(double v, Cell c, string info)
        {
            if (!c.IsNumericValue)
            {
                Assert.Fail(info + " Double value was required but actual was " + c.Value);
            }
            Assert.AreEqual(v, c.IntValue, info);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


