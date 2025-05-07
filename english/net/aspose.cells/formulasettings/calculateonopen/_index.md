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
// Called: workbook.Settings.FormulaSettings.CalculateOnOpen = false;
[Test]
        public void Property_CalculateOnOpen()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Duplicate3_3.xlsx");
            workbook.CalculateFormula(new CalculationOptions() { CustomEngine = new LookupCustomFunction() });
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            workbook.Settings.FormulaSettings.CalculateOnOpen = false;
            workbook.Save(Constants.destPath + "CellsNet31243.xlsx");
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


