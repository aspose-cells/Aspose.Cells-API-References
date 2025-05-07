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
// Called: if (data.FunctionName == "MYFUNC")
public override void Property_FunctionName(CalculationData data)
            {
                if (data.FunctionName == "MYFUNC")
                {
                    string text = data.GetParamText(0);
                    Name name = names[text];
                    if (name == null)
                    {
                        Assert.Fail("Cannot get corresponding Name object of " + text);
                    }
                    ProcessNamesForPerf(sn % 10 == 0 ? text + ": " : null, names, false);
                    data.CalculatedValue = sn;
                    sn++;
                }
            }
```

### See Also

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


