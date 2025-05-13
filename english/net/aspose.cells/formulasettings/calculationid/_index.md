---
title: FormulaSettings.CalculationId
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Specifies the version of the calculation engine used to calculate values in the workbook
type: docs
url: /net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

Specifies the version of the calculation engine used to calculate values in the workbook.

```csharp
public string CalculationId { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

### Examples

```csharp
// Called: wb.Settings.FormulaSettings.CalculationId = "181029";
public void FormulaSettings_Property_CalculationId()
{
    Workbook wb = new Workbook();
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    cell.Formula = "=AND(\"a\",true)";
    wb.CalculateFormula(false);
    Assert.AreEqual("#VALUE!", cell.Value, "Without CalculationId");
    wb.Settings.FormulaSettings.CalculationId = "181029";
    wb.CalculateFormula(false);
    Assert.AreEqual(true, cell.BoolValue, "With CalculationId 181029");
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


