---
title: WorkbookSettings.MaxColumn
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the max column index zerobased
type: docs
url: /net/aspose.cells/workbooksettings/maxcolumn/
---
## WorkbookSettings.MaxColumn property

Gets the max column index, zero-based.

```csharp
public int MaxColumn { get; }
```

### Remarks

Returns 255 if the file format is Excel97-2003;

### Examples

```csharp
// Called: Assert.AreEqual(16383, workbook.Settings.MaxColumn);
public void WorkbookSettings_Property_MaxColumn()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
   Assert.AreEqual(1048575,workbook.Settings.MaxRow);
   Assert.AreEqual(16383, workbook.Settings.MaxColumn);
    CellArea ca = CellArea.CreateCellArea("A","A");
    Assert.AreEqual(1048575, ca.EndRow);
    Assert.AreEqual(0, ca.EndColumn);
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


