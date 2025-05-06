---
title: FormulaSettings.CalculateOnOpen
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether the application is required to perform a full calculation when the workbook is opened
type: docs
url: /net/aspose.cells/formulasettings/calculateonopen/
---
## FormulaSettings.CalculateOnOpen property

Indicates whether the application is required to perform a full calculation when the workbook is opened.

```csharp
public bool CalculateOnOpen { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
// Called: wb.Settings.FormulaSettings.CalculateOnOpen = true;
[Test]
        public void Property_CalculateOnOpen()
        {
            var wb = new Workbook(Constants.sourcePath + &quot;Net53737.xlsx&quot;);
            Worksheet worksheet = wb.Worksheets[0];
            var ca = new CellArea();
            ca.StartRow = 10;
            ca.EndRow = 202;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // insert rows example
           // worksheet.Cells.InsertRows(10, 193, false);
            for (var r = 0; r &lt; 194; r++)
            {
                if (r &gt; 0)
                {
                    // copy styling and formulas
                    worksheet.Cells.CopyRow(worksheet.Cells, 9, 9 + r);
                }
            }
            Assert.AreEqual(1, worksheet.ConditionalFormattings.Count);
            Assert.AreEqual(1, worksheet.ConditionalFormattings[0].RangeCount);
            wb.Settings.FormulaSettings.CalculateOnOpen = true;
            wb = Util.ReSave(wb, SaveFormat.Xlsx);//wb.Save(Constants.destPath + &quot;Net53737_2.xlsx&quot;);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


