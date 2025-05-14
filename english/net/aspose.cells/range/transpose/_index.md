---
title: Range.Transpose
second_title: Aspose.Cells for .NET API Reference
description: Range method. Transpose rotate data from rows to columns or vice versa
type: docs
url: /net/aspose.cells/range/transpose/
---
## Range.Transpose method

Transpose (rotate) data from rows to columns or vice versa.

```csharp
public void Transpose()
```

### Examples

```csharp
// Called: c.Transpose();
public void Range_Method_Transpose()
{
    Workbook workbook = new Workbook(Constants.sourcePath + ("example.xlsx"));
    Aspose.Cells.Range c = workbook.Worksheets["Sheet4"].Cells.CreateRange("A1:C3");
    c.Transpose();
    Assert.AreEqual("6", workbook.Worksheets[3].Cells["B3"].StringValue);
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


