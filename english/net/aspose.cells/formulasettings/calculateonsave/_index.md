---
title: FormulaSettings.CalculateOnSave
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether recalculate the workbook before saving the document when in manual calculation mode
type: docs
url: /net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

Indicates whether recalculate the workbook before saving the document, when in manual calculation mode.

```csharp
public bool CalculateOnSave { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
// Called: Assert.IsTrue(workbook1.Settings.FormulaSettings.CalculateOnSave);//false
public void FormulaSettings_Property_CalculateOnSave()
{
    var workbook1 = new Workbook(Constants.sourcePath + "example.xlsx");
   Assert.IsTrue(workbook1.Settings.FormulaSettings.CalculateOnSave);//false
    var workbook2 = new Workbook(Constants.sourcePath + "example.xlsx");
   Assert.IsFalse(workbook2.Settings.FormulaSettings.CalculateOnSave);//false
                                                                                        
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


