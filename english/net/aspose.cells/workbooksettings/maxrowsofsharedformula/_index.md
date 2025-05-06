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
// Called: book.Settings.MaxRowsOfSharedFormula = 1024;
[Test]
        public void Property_MaxRowsOfSharedFormula()
        {
            Workbook book = new Workbook();
            book.Settings.MaxRowsOfSharedFormula = 100;
            Cells cells = book.Worksheets[0].Cells;
            cells[&quot;B1&quot;].SetSharedFormula(&quot;=A1&quot;, 101, 1);
            string f = (cells[&quot;B101&quot;].Formula);
            book.Worksheets.Add();
            book.Settings.MaxRowsOfSharedFormula = 1024;
            cells = book.Worksheets[1].Cells;
            cells[&quot;B1&quot;].SetSharedFormula(&quot;=A1&quot;, 101, 1);
            Assert.AreEqual(f, cells[&quot;B101&quot;].Formula);
            book.Save(Constants.destPath + &quot;CellsJava42510.xlsx&quot;);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


