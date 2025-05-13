---
title: Cell.IsMerged
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Checks if a cell is part of a merged range or not
type: docs
url: /net/aspose.cells/cell/ismerged/
---
## Cell.IsMerged property

Checks if a cell is part of a merged range or not.

```csharp
public bool IsMerged { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["A6"].IsMerged);
public void Cell_Property_IsMerged()
{
    Workbook data = new Workbook(Constants.sourcePath + "example.xlsx");
    DataTable dt = data.Worksheets[0].Cells.ExportDataTable(0, 0, 7, 5, true);

    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    WorkbookDesigner designer = new WorkbookDesigner(workbook);
    dt.TableName = "Level";
    designer.SetDataSource(dt);
    designer.Process();
    Assert.IsTrue(workbook.Worksheets[0].Cells["A6"].IsMerged);
    Assert.AreEqual(3, workbook.Worksheets[0].ConditionalFormattings[0].RangeCount);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


