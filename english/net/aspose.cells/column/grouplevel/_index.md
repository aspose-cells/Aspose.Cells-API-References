---
title: Column.GroupLevel
second_title: Aspose.Cells for .NET API Reference
description: Column property. Gets the group level of the column
type: docs
url: /net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

Gets the group level of the column.

```csharp
public byte GroupLevel { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells.Columns[0].GroupLevel, 0);
public void Column_Property_GroupLevel()
{
    Workbook workbook = new Workbook();
    workbook.Worksheets[0].Cells["A1"].PutValue("sdfsdfsdf");
    workbook.Worksheets[0].AutoFitColumns();
    workbook.Save(Constants.destPath + "GroupLevel0.xlsx");
    workbook = new Workbook(Constants.destPath + "GroupLevel0.xlsx");
    Assert.AreEqual(workbook.Worksheets[0].Cells.Columns[0].GroupLevel, 0);
}
```

### See Also

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


