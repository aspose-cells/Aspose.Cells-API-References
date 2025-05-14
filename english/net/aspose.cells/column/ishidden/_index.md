---
title: Column.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: Column property. Indicates whether the column is hidden
type: docs
url: /net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Indicates whether the column is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: workSheet.Cells.Columns[2].IsHidden = true;
public void Column_Property_IsHidden()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet  workSheet = workbook.Worksheets[0];
    double x = workSheet.Cells.Columns[2].Width;
    workSheet.Cells.Columns[2].IsHidden = true;

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(x, workbook.Worksheets[0].Cells.Columns[2].Width);


}
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


