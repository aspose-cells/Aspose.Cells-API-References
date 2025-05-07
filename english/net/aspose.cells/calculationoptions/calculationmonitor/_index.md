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
// Called: CalculationMonitor = new ForbidCircular()
[Test]
        public void Property_CalculationMonitor()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].Formula = "=1+A" + (i + 2);
            }
            cells[5, 0].Formula = "=1+B20";
            cells[0, 1].SetSharedFormula("=C1", 20, 1);
            cells[19, 2].Formula = "=1+B19";
            cells[18, 2].PutValue(1);
            cells[15, 2].Formula = "=1+A1";
            wb.CalculateFormula(new CalculationOptions()
            {
                CalcStackSize = 10,
                CalculationMonitor = new ForbidCircular()
            });
        }
```

### See Also

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


