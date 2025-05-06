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
// Called: Console.WriteLine(&amp;quot;Ignore calculation for [&amp;quot; + data.Worksheet.Index + &amp;quot;]&amp;quot;
public override void Property_Worksheet(CalculationData data)
        {
            if (_init)
            {
                _functions = new HashSet&lt;string&gt;();
                _init = false;
            }
            else if (_functions.Contains(data.FunctionName))
            {
                SkipCalculation();
                return;
            }
            _functions.Add(data.FunctionName);
            Console.WriteLine(&quot;Ignore calculation for [&quot; + data.Worksheet.Index + &quot;]&quot;
                + data.Worksheet.Name + &quot;!&quot; + CellsHelper.CellIndexToName(data.CellRow, data.CellColumn)
                + &quot;: &quot; + data.FunctionName);
            SkipCalculation();
        }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


