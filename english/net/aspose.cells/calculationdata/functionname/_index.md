---
title: CalculationData.FunctionName
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the function name to be calculated
type: docs
url: /net/aspose.cells/calculationdata/functionname/
---
## CalculationData.FunctionName property

Gets the function name to be calculated.

```csharp
public string FunctionName { get; }
```

### Examples

```csharp
// Called: if (data.FunctionName.ToLower().Equals(&amp;quot;hyperlink&amp;quot;))
public override void Property_FunctionName(CalculationData data)
            {
                if (data.FunctionName.ToLower().Equals(&quot;hyperlink&quot;))
                {
                    _invoked = true;
                    if (_processBuiltIn)
                    {
                        Assert.AreEqual(&quot;http://localhost:9090&quot;, data.GetParamValue(0), &quot;First parameter of HYPERLINK&quot;);
                        Assert.AreEqual(&quot;Target&quot;, data.GetParamValue(1), &quot;Second parameter of HYPERLINK&quot;);
                    }
                }
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


