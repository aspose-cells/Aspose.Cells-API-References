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
// Called: testAreEqual(null, cells[1, 2].Value, caseName);
private void Cell_Property_Value(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual("Product ID", cells[0, 0].StringValue, caseName);
            testAreEqual("Product Name", cells[0, 1].StringValue, caseName);
            testAreEqual(null, cells[0, 2].Value, caseName);
            testAreEqual(null, cells[1, 0].Value, caseName);
            testAreEqual(null, cells[1, 1].Value, caseName);
            testAreEqual(null, cells[1, 2].Value, caseName);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


