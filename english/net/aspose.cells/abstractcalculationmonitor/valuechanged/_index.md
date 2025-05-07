---
title: AbstractCalculationMonitor.ValueChanged
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationMonitor property. Whether the cells value has been changed after the calculation. Should be used only in AfterCalculate
type: docs
url: /net/aspose.cells/abstractcalculationmonitor/valuechanged/
---
## AbstractCalculationMonitor.ValueChanged property

Whether the cell's value has been changed after the calculation. Should be used only in [`AfterCalculate`](../aftercalculate/).

```csharp
public bool ValueChanged { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
public override void Property_ValueChanged(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }
```

### See Also

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


