---
title: ReferredArea.EndRow
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The end row of the area
type: docs
url: /net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

The end row of the area.

```csharp
public int EndRow { get; }
```

### Examples

```csharp
// Called: sb.Append(ra.EndRow + 1);
public override void Property_EndRow(CalculationData data)
            {
                string func = data.FunctionName.ToUpper();
                if ("USEDECIMAL".Equals(func))
                {
                    data.CalculatedValue = (decimal)(2.0 * (double)data.GetParamValue(0)); //using decimal for CELLSNET-44525
                }
                else if ("MULTIREF".Equals(func))
                {
                    object po = data.GetParamValue(0);
                    if (!(po is object[]))
                    {
                        data.CalculatedValue = "Unexpected parameter value type, should be object[] but was "
                            + po.GetType().FullName;
                        return;
                    }
                    object[] refs = (object[]) data.GetParamValue(0);
                    if (refs.Length != 3)
                    {
                        data.CalculatedValue = "Unexpected parameter value, array length should be 3 but was " + refs.Length;
                        return;
                    }
                    StringBuilder sb = new StringBuilder();
                    for (int i = 0; i < refs.Length; i++)
                    {
                        po = refs[i];
                        if (!(po is ReferredArea))
                        {
                            sb.Append(", Unexpected item type for parameter value, should be ReferredArea but was ");
                            sb.Append(po.GetType().FullName);
                            data.CalculatedValue = sb.ToString(1, sb.Length - 1);
                            return;
                        }
                        ReferredArea ra = (ReferredArea)po;
                        sb.Append(",$");
                        sb.Append(CellsHelper.ColumnIndexToName(ra.StartColumn));
                        sb.Append('$');
                        sb.Append(ra.StartRow + 1);
                        sb.Append(":$");
                        sb.Append(CellsHelper.ColumnIndexToName(ra.EndColumn));
                        sb.Append('$');
                        sb.Append(ra.EndRow + 1);
                    }
                    data.CalculatedValue = sb.ToString(1, sb.Length - 1);
                }
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


