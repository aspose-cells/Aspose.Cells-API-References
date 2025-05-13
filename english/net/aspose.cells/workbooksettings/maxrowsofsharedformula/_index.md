---
title: WorkbookSettings.MaxRowsOfSharedFormula
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets the max row number of shared formula
type: docs
url: /net/aspose.cells/workbooksettings/maxrowsofsharedformula/
---
## WorkbookSettings.MaxRowsOfSharedFormula property

Gets and sets the max row number of shared formula.

```csharp
public int MaxRowsOfSharedFormula { get; set; }
```

### Remarks

If the number is too large, the autofilter works very slow in MS Excel 2013.

### Examples

```csharp
// Called: book.Settings.MaxRowsOfSharedFormula = 100;
public void WorkbookSettings_Property_MaxRowsOfSharedFormula()
{
    Workbook book = new Workbook();
    book.Settings.MaxRowsOfSharedFormula = 100;
    Cells cells = book.Worksheets[0].Cells;
    cells["B1"].SetSharedFormula("=A1", 101, 1);
    string f = (cells["B101"].Formula);
    book.Worksheets.Add();
    book.Settings.MaxRowsOfSharedFormula = 1024;
    cells = book.Worksheets[1].Cells;
    cells["B1"].SetSharedFormula("=A1", 101, 1);
    Assert.AreEqual(f, cells["B101"].Formula);
    book.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


