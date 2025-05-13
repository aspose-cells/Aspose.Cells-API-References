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
// Called: Console.WriteLine("Value changed from [" + OriginalValue + "] to [" + CalculatedValue + "]");
public override void AbstractCalculationMonitor_Property_CalculatedValue(int sheetIndex, int rowIndex, int colIndex)
            {
                if (ValueChanged)
                {
                    Changed = true;
                    Console.WriteLine("Value changed from [" + OriginalValue + "] to [" + CalculatedValue + "]");
                }
            }
```

### See Also

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


