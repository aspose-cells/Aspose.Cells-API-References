---
title: Row.GroupLevel
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the group level of the row
type: docs
url: /net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Gets the group level of the row.

```csharp
public byte GroupLevel { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, workbook.Worksheets[0].Cells.Rows[4].GroupLevel);
public void Row_Property_GroupLevel()
{
    Workbook workbook = new Workbook(Constants.HtmlSourcePath + "CellsNet52159.mht");
    Assert.AreEqual(1, workbook.Worksheets[0].Cells.Rows[4].GroupLevel);

}
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


