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
// Called: Console.WriteLine(&amp;quot;Value changed from [&amp;quot; + OriginalValue + &amp;quot;] to [&amp;quot; + CalculatedValue + &amp;quot;]&amp;quot;);
public override void Property_OriginalValue(int sheetIndex, int rowIndex, int colIndex)
            {
                if (ValueChanged)
                {
                    Changed = true;
                    Console.WriteLine(&quot;Value changed from [&quot; + OriginalValue + &quot;] to [&quot; + CalculatedValue + &quot;]&quot;);
                }
            }
```

### See Also

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


