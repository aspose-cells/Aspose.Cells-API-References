---
title: FormulaSettings.PrecisionAsDisplayed
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Whether the precision of calculated result be set as they are displayed while calculating formulas
type: docs
url: /net/aspose.cells/formulasettings/precisionasdisplayed/
---
## FormulaSettings.PrecisionAsDisplayed property

Whether the precision of calculated result be set as they are displayed while calculating formulas

```csharp
public bool PrecisionAsDisplayed { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.FormulaSettings.PrecisionAsDisplayed = false;
[Test, Category("Bug")]
        public void Property_PrecisionAsDisplayed()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.FormulaSettings.PrecisionAsDisplayed = false;
            Cells cells = workbook.Worksheets[0].Cells;
            string formula = "=SUM('C:\\[Data.xls]Sheet1'!A1:A5)".ToUpper();
            cells["A1"].Formula = formula;
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells["A1"].Formula, formula);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


