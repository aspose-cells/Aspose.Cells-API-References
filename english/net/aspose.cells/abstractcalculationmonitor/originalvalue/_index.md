---
title: AbstractCalculationMonitor.OriginalValue
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationMonitor property. Gets the old value of the calculated cell. Should be used only in BeforeCalculate and AfterCalculate
type: docs
url: /net/aspose.cells/abstractcalculationmonitor/originalvalue/
---
## AbstractCalculationMonitor.OriginalValue property

Gets the old value of the calculated cell. Should be used only in [`BeforeCalculate`](../beforecalculate/) and [`AfterCalculate`](../aftercalculate/).

```csharp
public object OriginalValue { get; }
```

### Examples

```csharp
// Called: Console.WriteLine("Value changed from [" + OriginalValue + "] to [" + CalculatedValue + "]");
public override void AbstractCalculationMonitor_Property_OriginalValue(int sheetIndex, int rowIndex, int colIndex)
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


