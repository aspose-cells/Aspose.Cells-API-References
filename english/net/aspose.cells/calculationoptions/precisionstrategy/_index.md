---
title: CalculationOptions.PrecisionStrategy
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Specifies the strategy for processing precision of calculation
type: docs
url: /net/aspose.cells/calculationoptions/precisionstrategy/
---
## CalculationOptions.PrecisionStrategy property

Specifies the strategy for processing precision of calculation.

```csharp
public CalculationPrecisionStrategy PrecisionStrategy { get; set; }
```

### Examples

```csharp
// Called: copt.PrecisionStrategy = CalculationPrecisionStrategy.None; //Decimal and Round cannot give correct value
[Test]
        public void Property_PrecisionStrategy()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].Formula = &quot;=57750/4500&quot;;
            cells[0, 1].Formula = &quot;=A1*4500&quot;;
            CalculationOptions copt = new CalculationOptions();
            copt.PrecisionStrategy = CalculationPrecisionStrategy.None; //Decimal and Round cannot give correct value

            workbook.CalculateFormula(copt);
            Assert.AreEqual(cells[&quot;B1&quot;].DoubleValue, 57750);

            workbook = new Workbook(Constants.sourcePath + &quot;Formula/CELLSNET-40120.xls&quot;);
            workbook.CalculateFormula(copt);
            Assert.AreEqual(workbook.Worksheets[&quot;rekenblad&quot;].Cells[&quot;A22&quot;].DoubleValue, 57750);
        }
```

### See Also

* enum [CalculationPrecisionStrategy](../../calculationprecisionstrategy/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


