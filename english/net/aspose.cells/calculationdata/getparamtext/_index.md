---
title: CalculationData.GetParamText
second_title: Aspose.Cells for .NET API Reference
description: CalculationData method. Gets the literal text of the parameter at given index
type: docs
url: /net/aspose.cells/calculationdata/getparamtext/
---
## CalculationData.GetParamText method

Gets the literal text of the parameter at given index.

```csharp
public string GetParamText(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | index of the parameter(0 based) |

### Return Value

literal text of the parameter

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;B1+B1&amp;quot;, data.GetParamText(0));
public override void Method_Int32_(CalculationData data)
            {
                Assert.AreEqual(&quot;B1+B1&quot;, data.GetParamText(0));
                Assert.AreEqual(&quot;C1:C5&quot;, data.GetParamText(1));
                Assert.AreEqual(&quot;SUM(\&quot;test\&quot;)&quot;, data.GetParamText(2));
                data.CalculatedValue = 0;
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


