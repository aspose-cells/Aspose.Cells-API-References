---
title: WorkbookSettings.CultureInfo
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets or sets the system culture info
type: docs
url: /net/aspose.cells/workbooksettings/cultureinfo/
---
## WorkbookSettings.CultureInfo property

Gets or sets the system culture info.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Remarks

Returns null if culture info is not set and [`Region`](../region/) is not set.

### Examples

```csharp
// Called: excelCalc.Settings.CultureInfo = ci;
public static void Property_CultureInfo(Workbook excelCalc, CalculationOptions opts, CultureInfo ci)
        {
            if (ci != null)
            {
                excelCalc.Settings.CultureInfo = ci;
            }
            //excelCalc.ClearFormulaValues();
            excelCalc.RefreshDynamicArrayFormulas(true, opts);
            excelCalc.CalculateFormula(opts);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


