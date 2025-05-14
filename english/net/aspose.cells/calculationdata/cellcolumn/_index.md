---
title: CalculationData.CellColumn
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the column index of the cell where the function is in
type: docs
url: /net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Gets the column index of the cell where the function is in.

```csharp
public int CellColumn { get; }
```

### Examples

```csharp
// Called: _values[data.CellColumn] = data.CalculatedValue;
public override void CalculationData_Property_CellColumn(CalculationData data)
            {
                if (_values == null)
                {
                    throw new Exception("Custom implementation to ignore calculation of formula with function "
                        + data.FunctionName);
                }
                _values[data.CellColumn] = data.CalculatedValue;
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


