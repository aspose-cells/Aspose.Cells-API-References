---
title: ReferredArea.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The start column of the area
type: docs
url: /net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

The start column of the area.

```csharp
public int StartColumn { get; }
```

### Examples

```csharp
// Called: sb.Append(CellsHelper.ColumnIndexToName(ra.StartColumn));
public override void Property_StartColumn(CalculationData data)
            {
                string func = data.FunctionName.ToUpper();
                if (&quot;USEDECIMAL&quot;.Equals(func))
                {
                    data.CalculatedValue = (decimal)(2.0 * (double)data.GetParamValue(0)); //using decimal for CELLSNET-44525
                }
                else if (&quot;MULTIREF&quot;.Equals(func))
                {
                    object po = data.GetParamValue(0);
                    if (!(po is object[]))
                    {
                        data.CalculatedValue = &quot;Unexpected parameter value type, should be object[] but was &quot;
                            + po.GetType().FullName;
                        return;
                    }
                    object[] refs = (object[]) data.GetParamValue(0);
                    if (refs.Length != 3)
                    {
                        data.CalculatedValue = &quot;Unexpected parameter value, array length should be 3 but was &quot; + refs.Length;
                        return;
                    }
                    StringBuilder sb = new StringBuilder();
                    for (int i = 0; i &lt; refs.Length; i++)
                    {
                        po = refs[i];
                        if (!(po is ReferredArea))
                        {
                            sb.Append(&quot;, Unexpected item type for parameter value, should be ReferredArea but was &quot;);
                            sb.Append(po.GetType().FullName);
                            data.CalculatedValue = sb.ToString(1, sb.Length - 1);
                            return;
                        }
                        ReferredArea ra = (ReferredArea)po;
                        sb.Append(&quot;,$&quot;);
                        sb.Append(CellsHelper.ColumnIndexToName(ra.StartColumn));
                        sb.Append(&apos;$&apos;);
                        sb.Append(ra.StartRow + 1);
                        sb.Append(&quot;:$&quot;);
                        sb.Append(CellsHelper.ColumnIndexToName(ra.EndColumn));
                        sb.Append(&apos;$&apos;);
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


