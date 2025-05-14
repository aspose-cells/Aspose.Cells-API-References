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
// Called: + data.Worksheet.Name + "!" + CellsHelper.CellIndexToName(data.CellRow, data.CellColumn)
public override void CalculationData_Property_CellRow(CalculationData data)
        {
            if (_init)
            {
                _functions = new HashSet<string>();
                _init = false;
            }
            else if (_functions.Contains(data.FunctionName))
            {
                SkipCalculation();
                return;
            }
            _functions.Add(data.FunctionName);
            Console.WriteLine("Ignore calculation for [" + data.Worksheet.Index + "]"
                + data.Worksheet.Name + "!" + CellsHelper.CellIndexToName(data.CellRow, data.CellColumn)
                + ": " + data.FunctionName);
            SkipCalculation();
        }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


