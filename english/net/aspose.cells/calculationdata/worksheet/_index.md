---
title: CalculationData.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the Worksheet object where the function is in
type: docs
url: /net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Gets the Worksheet object where the function is in.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: data.CalculatedValue = data.Worksheet.CalculateArrayFormula(
public override void CalculationData_Property_Worksheet(CalculationData data)
            {
                CellRow = data.CellRow;
                CellColumn = data.CellColumn;
                BaseCell = data.Cell;

                data.CalculatedValue = data.Worksheet.CalculateArrayFormula(
                    "=IFERROR(A2:A4,B2:B4)", new CalculationOptions());
            }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


