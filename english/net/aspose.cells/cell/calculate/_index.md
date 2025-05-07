---
title: Cell.Calculate
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Calculates the formula of the cell
type: docs
url: /net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Calculates the formula of the cell.

```csharp
public void Calculate(CalculationOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| options | CalculationOptions | Options for calculation |

### Examples

```csharp
// Called: cell.Calculate(new CalculationOptions());
[Test]
        public void Method_CalculationOptions_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            for (int i = 0; i < 3; i++)
            {
                cells[i, 0].PutValue(i);
                cells[0, i].PutValue(i);
            }
            cells[3, 0].PutValue(3);
            Cell cell = cells[1, 1];
            cell.Formula = "=MMULT(A1:D1,A1:A4)";
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual("#VALUE!", cell.Value);

            cells[0, 3].PutValue(3);
            cells[0, 4].PutValue(4);
            cell.Formula = "=MMULT(A1:E1,A1:A5)";
            cell.Calculate(new CalculationOptions());
            Assert.AreEqual("#VALUE!", cell.Value);
        }
```

### See Also

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


