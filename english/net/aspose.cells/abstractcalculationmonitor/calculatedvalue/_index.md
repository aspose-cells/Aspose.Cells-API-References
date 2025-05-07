---
title: AbstractCalculationMonitor.CalculatedValue
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationMonitor property. Gets the newly calculated value of the cell. Should be used only in AfterCalculate
type: docs
url: /net/aspose.cells/abstractcalculationmonitor/calculatedvalue/
---
## AbstractCalculationMonitor.CalculatedValue property

Gets the newly calculated value of the cell. Should be used only in [`AfterCalculate`](../aftercalculate/).

```csharp
public object CalculatedValue { get; }
```

### Examples

```csharp
// Called: Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
public override void Property_CalculatedValue(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }
```

### See Also

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


