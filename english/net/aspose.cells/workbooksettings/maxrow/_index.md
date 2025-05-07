---
title: WorkbookSettings.MaxRow
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the max row index zerobased
type: docs
url: /net/aspose.cells/workbooksettings/maxrow/
---
## WorkbookSettings.MaxRow property

Gets the max row index, zero-based.

```csharp
public int MaxRow { get; }
```

### Remarks

Returns 65535 if the file format is Excel97-2003;

### Examples

```csharp
// Called: Assert.AreEqual(1048575,workbook.Settings.MaxRow);
[Test]
        public void Property_MaxRow()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Cell44388.xlsx");
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


