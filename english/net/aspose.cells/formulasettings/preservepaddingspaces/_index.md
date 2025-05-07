---
title: FormulaSettings.PreservePaddingSpaces
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
type: docs
url: /net/aspose.cells/formulasettings/preservepaddingspaces/
---
## FormulaSettings.PreservePaddingSpaces property

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```csharp
public bool PreservePaddingSpaces { get; set; }
```

### Remarks

Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.

### Examples

```csharp
// Called: AssertHelper.AreEqual(wb.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(" ", ""),
[Test]
        public void Property_PreservePaddingSpaces()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "IfErrorIssue.xlsb");
            string fml = "=IFERROR(A1, 0)";
            AssertHelper.AreEqual(wb.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(" ", ""),
                wb.Worksheets[0].Cells[1, 0].Formula, "A2's formula");
            wb.Save(Constants.checkPath + "IfErrorIssue_res.xlsx");
            wb = new Workbook(Constants.checkPath + "IfErrorIssue_res.xlsx");
            AssertHelper.AreEqual(wb.Settings.FormulaSettings.PreservePaddingSpaces ? fml : fml.Replace(" ", ""),
                wb.Worksheets[0].Cells[1, 0].Formula, "A2's formula");
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


