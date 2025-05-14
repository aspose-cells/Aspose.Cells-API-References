---
title: Row.IsHidden
second_title: Aspose.Cells for .NET API Reference
description: Row property. Indicates whether the row is hidden
type: docs
url: /net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Indicates whether the row is hidden.

```csharp
public bool IsHidden { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, cells.Rows[999].IsHidden);
public void Row_Property_IsHidden()
{
    //Row Hidden and formula(range) error
    Workbook wb = new Workbook(Constants.sourcePath + "example.numbers");
    //wb.Save(Constants.destPath + @"example.xlsx");
    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("1260", cells["D73"].StringValue);
    Assert.AreEqual("=SUM(D5:D72)", cells["D73"].Formula);
    Assert.AreEqual("R$10,509.48", cells["E73"].StringValue);
    Assert.AreEqual("=SUM(E5:E72)", cells["E73"].Formula);
    Assert.AreEqual(true, cells.Rows[0].IsHidden);
    Assert.AreEqual(true, cells.Rows[1].IsHidden);
    Assert.AreEqual(true, cells.Rows[2].IsHidden);
    Assert.AreEqual(true, cells.Rows[3].IsHidden);
    Assert.AreEqual(false, cells.Rows[4].IsHidden);
    Assert.AreEqual(true, cells.Rows[11].IsHidden);
    Assert.AreEqual(true, cells.Rows[12].IsHidden);
    Assert.AreEqual(false, cells.Rows[13].IsHidden);
    Assert.AreEqual(false, cells.Rows[14].IsHidden);
    Assert.AreEqual(true, cells.Rows[27].IsHidden);
    Assert.AreEqual(true, cells.Rows[52].IsHidden);
    Assert.AreEqual(true, cells.Rows[55].IsHidden);
    Assert.AreEqual(false, cells.Rows[57].IsHidden);
    Assert.AreEqual(true, cells.Rows[999].IsHidden);
    Assert.AreEqual("R$1,501.35", cells["E1008"].StringValue);

}
```

### See Also

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


