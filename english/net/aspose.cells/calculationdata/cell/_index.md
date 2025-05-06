---
title: CalculationData.Cell
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the Cell object where the function is in
type: docs
url: /net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Gets the Cell object where the function is in.

```csharp
public Cell Cell { get; }
```

### Remarks

When calculating a formula without setting it to a cell, such as by [`CalculateFormula`](../../worksheet/calculateformula/), the formula will be calculated just like it has been set to cell A1, so both [`CellRow`](../cellrow/) and [`CellColumn`](../cellcolumn/) are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.

### Examples

```csharp
// Called: BaseCell = data.Cell;
public override void Property_Cell(CalculationData data)
            {
                CellRow = data.CellRow;
                CellColumn = data.CellColumn;
                BaseCell = data.Cell;

                data.CalculatedValue = data.Worksheet.CalculateArrayFormula(
                    &quot;=IFERROR(A2:A4,B2:B4)&quot;, new CalculationOptions());
            }
```

### See Also

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


