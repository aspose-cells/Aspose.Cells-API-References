---
title: AutoFilter.SetRange
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter method. Sets the range to which the specified AutoFilter applies
type: docs
url: /net/aspose.cells/autofilter/setrange/
---
## AutoFilter.SetRange method

Sets the range to which the specified AutoFilter applies.

```csharp
public void SetRange(int row, int startColumn, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| startColumn | Int32 | Start column index. |
| endColumn | Int32 | End column Index. |

### Examples

```csharp
// Called: sheet.AutoFilter.SetRange(0, 0, 1);
public void AutoFilter_Method_SetRange()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet sheet = workbook.Worksheets[0];
    sheet.AutoFilter.SetRange(0, 0, 1);
    sheet.AutoFilter.Custom(1,FilterOperatorType.Equal, "R?C2");
    sheet.AutoFilter.Refresh();
    Util.ReSave(workbook, SaveFormat.Excel97To2003); //.Save(Constants.destPath + "example.xls");
    Assert.AreEqual(sheet.Cells.GetRowHeight(3), 0);
    Assert.AreEqual(sheet.Cells.GetRowHeight(4), 12.75);
}
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


