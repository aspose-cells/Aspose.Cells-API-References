---
title: WorkbookSettings.FormulaSettings
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets the settings for formularelated features
type: docs
url: /net/aspose.cells/workbooksettings/formulasettings/
---
## WorkbookSettings.FormulaSettings property

Gets the settings for formula-related features.

```csharp
public FormulaSettings FormulaSettings { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CalcModeType.Manual, wb1.Settings.FormulaSettings.CalculationMode, "Copied CalcMode");
public void WorkbookSettings_Property_FormulaSettings()
{
    Workbook wb = new Workbook();
    wb.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
    Workbook wb1 = new Workbook();
    wb1.Copy(wb);
    Assert.AreEqual(CalcModeType.Manual, wb1.Settings.FormulaSettings.CalculationMode, "Copied CalcMode");
}
```

### See Also

* class [FormulaSettings](../../formulasettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


