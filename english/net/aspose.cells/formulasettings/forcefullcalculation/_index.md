---
title: FormulaSettings.ForceFullCalculation
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether calculates all formulas every time when a calculation is triggered
type: docs
url: /net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

Indicates whether calculates all formulas every time when a calculation is triggered.

```csharp
public bool ForceFullCalculation { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
// Called: formulaSettings.ForceFullCalculation = false;
public static void FormulaSettings_Property_ForceFullCalculation()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the workbook's formula settings
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // Setting properties
            formulaSettings.CalculateOnOpen = true;
            formulaSettings.CalculateOnSave = true;
            formulaSettings.ForceFullCalculation = false;
            formulaSettings.CalculationMode = CalcModeType.Automatic;
            formulaSettings.CalculationId = "0";
            formulaSettings.EnableIterativeCalculation = true;
            formulaSettings.MaxIteration = 100;
            formulaSettings.MaxChange = 0.001;
            formulaSettings.PrecisionAsDisplayed = false;
            formulaSettings.EnableCalculationChain = true;
            formulaSettings.PreservePaddingSpaces = false;

            // Save the workbook
            workbook.Save("FormulaSettingsExample.xlsx");
            workbook.Save("FormulaSettingsExample.pdf");
            return;
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


