---
title: Workbook.Settings
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Represents the workbook settings
type: docs
url: /net/aspose.cells/workbook/settings/
---
## Workbook.Settings property

Represents the workbook settings.

```csharp
public WorkbookSettings Settings { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(CalcModeType.Manual, wb1.Settings.FormulaSettings.CalculationMode, &amp;quot;Copied CalcMode&amp;quot;);
[Test]
        public void Property_Settings()
        {
            Workbook wb = new Workbook();
            wb.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Workbook wb1 = new Workbook();
            wb1.Copy(wb);
            Assert.AreEqual(CalcModeType.Manual, wb1.Settings.FormulaSettings.CalculationMode, &quot;Copied CalcMode&quot;);
        }
```

### See Also

* class [WorkbookSettings](../../workbooksettings/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


