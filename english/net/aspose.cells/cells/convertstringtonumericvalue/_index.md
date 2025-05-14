---
title: Cells.ConvertStringToNumericValue
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Converts all string data in the worksheet to numeric value if possible
type: docs
url: /net/aspose.cells/cells/convertstringtonumericvalue/
---
## Cells.ConvertStringToNumericValue method

Converts all string data in the worksheet to numeric value if possible.

```csharp
public void ConvertStringToNumericValue()
```

### Examples

```csharp
// Called: cells.ConvertStringToNumericValue();
public void Cells_Method_ConvertStringToNumericValue()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells[0, 0].PutValue("1.23");
    cells[0, 1].PutValue("1.24");
    cells[0, 2].PutValue("1.23");
    cells[0, 3].PutValue("6/20/2021");
    cells[0, 4].PutValue("def");
    cells[0, 5].PutValue("6/20/2021");
    cells.ConvertStringToNumericValue();
    Assert.AreEqual(1.23, cells[0, 0].DoubleValue, "A1");
    Assert.AreEqual(1.24, cells[0, 1].DoubleValue, "B1");
    Assert.AreEqual(1.23, cells[0, 2].DoubleValue, "C1");
    Assert.AreEqual(44367.0, cells[0, 3].DoubleValue, "D1");
    Assert.AreEqual(44367.0, cells[0, 5].DoubleValue, "D1");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


