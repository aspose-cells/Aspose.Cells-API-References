---
title: CalculationOptions.CalcStackSize
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. The stack size for calculating cells recursively. Default value is 200
type: docs
url: /net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

The stack size for calculating cells recursively. Default value is 200.

```csharp
public int CalcStackSize { get; set; }
```

### Remarks

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### Examples

```csharp
// Called: wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 100 });
[Test]
        public void Property_CalcStackSize()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            cells["A1"].PutValue(1);
            int last = 800;
            cells["B1"].Formula = "=A" + last + "-A2";
            cells["C1"].Formula = "=B" + last + "-B2";
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=0.8 * A" + (i - 1);
                cells["B" + i].Formula = "=0.8 * B" + (i + 1);
            }
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 100 });
        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


