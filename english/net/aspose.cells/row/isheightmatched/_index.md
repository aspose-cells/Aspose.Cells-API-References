---
title: Row.IsHeightMatched
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is automatic without custom height value set by user
type: docs
url: /net/aspose.cells/row/isheightmatched/
---
## Row.IsHeightMatched property

Indicates whether the row height matches current default font setting of the workbook. True of this property also denotes the row height is "automatic" without custom height value set by user.

```csharp
public bool IsHeightMatched { get; set; }
```

### Remarks

When this property is true, if the content in this row changes, generally the row height needs to be re-calculated(such as by [`AutoFitRows`](../../worksheet/autofitrows/)) to get the same result with what is shown in ms excel when you opening the workbook in it.

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells.Rows[0].IsHeightMatched,true);
public void Row_Property_IsHeightMatched()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "autofitcells.xlsx");
    workbook.Worksheets[0].AutoFitRows();
    Assert.AreEqual(workbook.Worksheets[0].Cells.Rows[0].IsHeightMatched,true);
}
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


