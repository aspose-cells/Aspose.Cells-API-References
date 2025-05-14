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
// Called: if (data.ParamCount < 6)
public override void CalculationData_Property_ParamCount(CalculationData data)
            {
                if (data.ParamCount < 6)
                {
                    Assert.Fail(mMsgHeader
                        + "Count of the arguments that provided to user's engine for STOCKHISTORY should not be less than 6");
                }
                int iv = GetValue(data.GetParamValue(1));
                double[][] expected;
                if (data.ParamCount > 6)
                {
                    Assert.AreEqual(0, GetValue(data.GetParamValue(3)), mMsgHeader + "Interval");
                    Assert.AreEqual(1, GetValue(data.GetParamValue(4)), mMsgHeader + "Headers");
                    Assert.AreEqual(0, GetValue(data.GetParamValue(5)), mMsgHeader + "Retrieved column 0");
                    Assert.AreEqual(1, GetValue(data.GetParamValue(6)), mMsgHeader + "Retrieved column 1");
                    expected = new double[GetValue(data.GetParamValue(2)) - iv + 1][];
                }
                else
                {
                    Assert.AreEqual(1, GetValue(data.GetParamValue(3)), mMsgHeader + "Interval");
                    Assert.AreEqual(0, GetValue(data.GetParamValue(4)), mMsgHeader + "Headers");
                    Assert.AreEqual(2, GetValue(data.GetParamValue(5)), mMsgHeader + "Retrieved column 0");
                    expected = new double[GetValue(data.GetParamValue(2)) - iv + 5][];
                }
                for (int i = 0; i < expected.Length; i++)
                {
                    expected[i] = data.ParamCount > 6 ? new double[] { iv + i, 100.0 + i / 10.0 } : new double[] { iv + i };
                }
                data.CalculatedValue = expected;
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


