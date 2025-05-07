---
title: Cell.DateTimeValue
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the DateTime value contained in the cell
type: docs
url: /net/aspose.cells/cell/datetimevalue/
---
## Cell.DateTimeValue property

Gets the DateTime value contained in the cell.

```csharp
public DateTime DateTimeValue { get; }
```

### Examples

```csharp
// Called: testAreEqual(new DateTime(2009, 9, 2), cells[2, 0].DateTimeValue, caseName);
private void Property_DateTimeValue(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            testAreEqual("Product ID", cells[0, 0].StringValue, caseName);
            testAreEqual(new DateTime(2009, 9, 1), cells[1, 0].DateTimeValue, caseName);
            testAreEqual("dd/mm/yy", cells[1, 0].GetStyle().Custom, caseName);
            testAreEqual(new DateTime(2009, 9, 2), cells[2, 0].DateTimeValue, caseName);
            testAreEqual("dd/mm/yy", cells[2, 0].GetStyle().Custom, caseName);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


