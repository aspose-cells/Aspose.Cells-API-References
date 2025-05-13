---
title: Cell.GetConditionalFormattingResult
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Get the result of the conditional formatting
type: docs
url: /net/aspose.cells/cell/getconditionalformattingresult/
---
## Cell.GetConditionalFormattingResult method

Get the result of the conditional formatting.

```csharp
public ConditionalFormattingResult GetConditionalFormattingResult()
```

### Remarks

Returns null if no conditional formatting is applied to this cell,

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells["H12"].GetConditionalFormattingResult().ConditionalStyle != null, true);
public void Cell_Method_GetConditionalFormattingResult()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].Cells.InsertRows(11, 2);
    workbook.Worksheets[0].Cells.CopyRows(workbook.Worksheets[0].Cells, 8, 10, 2);
    Assert.AreEqual(workbook.Worksheets[0].Cells["H12"].GetConditionalFormattingResult().ConditionalStyle != null, true);
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [ConditionalFormattingResult](../../conditionalformattingresult/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


