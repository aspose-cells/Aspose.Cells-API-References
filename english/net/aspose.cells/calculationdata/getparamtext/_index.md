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
// Called: data.GetParamText(0), sn + ": SUM's parameter");
public override void Method_Int32_(CalculationData data)
            {
                sn++;
                if (data.FunctionName == "SUM")
                {
                    Assert.AreEqual(sn == 1 ? "Book2.xlsx!Table1[#All]"
                        : "INDIRECT(\"'Book2.xlsx'!Table1[#All]\")",
                        data.GetParamText(0), sn + ": SUM's parameter");
                }
                else if (data.FunctionName == "INDIRECT")
                {
                    Assert.AreEqual("\"'Book2.xlsx'!Table1[#All]\"",
                        data.GetParamText(0), sn + ": INDIRECT's parameter");
                }
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


