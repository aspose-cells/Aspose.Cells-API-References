---
title: CalculationData.CellRow
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the row index of the cell where the function is in
type: docs
url: /net/aspose.cells/calculationdata/cellrow/
---
## CalculationData.CellRow property

Gets the row index of the cell where the function is in.

```csharp
public int CellRow { get; }
```

### Examples

```csharp
// Called: CellRow = data.CellRow;
public override void Property_CellRow(CalculationData data)
            {
                CellRow = data.CellRow;
                CellColumn = data.CellColumn;
                BaseCell = data.Cell;

                data.CalculatedValue = data.Worksheet.CalculateArrayFormula(
                    "=IFERROR(A2:A4,B2:B4)", new CalculationOptions());
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


