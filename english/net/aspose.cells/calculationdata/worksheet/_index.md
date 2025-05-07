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
// Called: + data.Worksheet.Name + "!" + CellsHelper.CellIndexToName(data.CellRow, data.CellColumn)
public override void Property_Worksheet(CalculationData data)
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

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


