---
title: CalculationData.ParamCount
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the count of parameters
type: docs
url: /net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Gets the count of parameters

```csharp
public int ParamCount { get; }
```

### Examples

```csharp
// Called: if (data.ParamCount &amp;lt; 6)
public override void Property_ParamCount(CalculationData data)
            {
                if (data.ParamCount &lt; 6)
                {
                    Assert.Fail(mMsgHeader
                        + &quot;Count of the arguments that provided to user&apos;s engine for STOCKHISTORY should not be less than 6&quot;);
                }
                int iv = GetValue(data.GetParamValue(1));
                double[][] expected;
                if (data.ParamCount &gt; 6)
                {
                    Assert.AreEqual(0, GetValue(data.GetParamValue(3)), mMsgHeader + &quot;Interval&quot;);
                    Assert.AreEqual(1, GetValue(data.GetParamValue(4)), mMsgHeader + &quot;Headers&quot;);
                    Assert.AreEqual(0, GetValue(data.GetParamValue(5)), mMsgHeader + &quot;Retrieved column 0&quot;);
                    Assert.AreEqual(1, GetValue(data.GetParamValue(6)), mMsgHeader + &quot;Retrieved column 1&quot;);
                    expected = new double[GetValue(data.GetParamValue(2)) - iv + 1][];
                }
                else
                {
                    Assert.AreEqual(1, GetValue(data.GetParamValue(3)), mMsgHeader + &quot;Interval&quot;);
                    Assert.AreEqual(0, GetValue(data.GetParamValue(4)), mMsgHeader + &quot;Headers&quot;);
                    Assert.AreEqual(2, GetValue(data.GetParamValue(5)), mMsgHeader + &quot;Retrieved column 0&quot;);
                    expected = new double[GetValue(data.GetParamValue(2)) - iv + 5][];
                }
                for (int i = 0; i &lt; expected.Length; i++)
                {
                    expected[i] = data.ParamCount &gt; 6 ? new double[] { iv + i, 100.0 + i / 10.0 } : new double[] { iv + i };
                }
                data.CalculatedValue = expected;
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


