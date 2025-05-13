---
title: Worksheet.GetPanes
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Gets the window panes
type: docs
url: /net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Gets the window panes.

```csharp
public PaneCollection GetPanes()
```

### Remarks

If the window is not split or frozen.

### Examples

```csharp
// Called: Assert.AreEqual(2,workbook.Worksheets[0].GetPanes().FirstVisibleRowOfBottomPane);
public void Worksheet_Method_GetPanes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].Cells.DeleteRow(0);
    Assert.AreEqual(2,workbook.Worksheets[0].GetPanes().FirstVisibleRowOfBottomPane);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


