---
title: Class FormulaSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FormulaSettings class. Settings of formulas and calculation
type: docs
url: /net/aspose.cells/formulasettings/
---
## FormulaSettings class

Settings of formulas and calculation.

```csharp
public class FormulaSettings
```

## Properties

| Name | Description |
| --- | --- |
| [CalculateOnOpen](../../aspose.cells/formulasettings/calculateonopen/) { get; set; } | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [CalculateOnSave](../../aspose.cells/formulasettings/calculateonsave/) { get; set; } | Indicates whether to recalculate the workbook before saving the document, when in manual calculation mode. |
| [CalculationId](../../aspose.cells/formulasettings/calculationid/) { get; set; } | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [CalculationMode](../../aspose.cells/formulasettings/calculationmode/) { get; set; } | Gets or sets the mode for workbook calculation in MS Excel. |
| [EnableCalculationChain](../../aspose.cells/formulasettings/enablecalculationchain/) { get; set; } | Indicates whether to enable calculation chain for formulas. Default is false. |
| [EnableIterativeCalculation](../../aspose.cells/formulasettings/enableiterativecalculation/) { get; set; } | Indicates whether to enable iterative calculation to resolve circular references. |
| [ForceFullCalculation](../../aspose.cells/formulasettings/forcefullcalculation/) { get; set; } | Indicates whether it calculates all formulas every time when a calculation is triggered. |
| [MaxChange](../../aspose.cells/formulasettings/maxchange/) { get; set; } | The maximum change to resolve a circular reference. |
| [MaxIteration](../../aspose.cells/formulasettings/maxiteration/) { get; set; } | The maximum iterations to resolve a circular reference. |
| [PrecisionAsDisplayed](../../aspose.cells/formulasettings/precisionasdisplayed/) { get; set; } | Indicates whether the precision of calculated result be set as they are displayed while calculating formulas. |
| [PreservePaddingSpaces](../../aspose.cells/formulasettings/preservepaddingspaces/) { get; set; } | Indicates whether to preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormulaSettingsDemo
    {
        public static void FormulaSettingsExample()
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
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


