---
title: CalculationOptions.CalculationMonitor
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. The monitor for user to track the progress of formula calculation
type: docs
url: /net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

The monitor for user to track the progress of formula calculation.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### Examples

```csharp
// Called: copts.CalculationMonitor = new CheckStackCalculationMonitor();
        public void CalculationOptions_Property_CalculationMonitor()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
            wb.Worksheets["Satteldachbinder"].Cells["J9"].Value = 2600;
            CalculationOptions copts = new CalculationOptions();
#if NETCOREAPP2_0
            copts.CalcStackSize = 100;
#endif
            copts.CalculationMonitor = new CheckStackCalculationMonitor();
            wb.CalculateFormula(copts);
        }
```

### See Also

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


