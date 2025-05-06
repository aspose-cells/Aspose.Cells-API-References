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
// Called: int rc = ra.EndRow - ra.StartRow + 1;
public override void Property_EndRow(CalculationData data)
            {
                if (data.FunctionName == &quot;MYFUNC&quot;)
                {
                    data.CalculatedValue = Indicator;
                }
                else
                {
                    for (int i = data.ParamCount - 1; i &gt; -1; i--)
                    {
                        object v = data.GetParamValue(i);
                        bool isBreak = false;
                        if (v is object[][])
                        {
                            foreach (object[] vr in (object[][])v)
                            {
                                foreach (object vi in vr)
                                {
                                    if (IsBreak(vi))
                                    {
                                        isBreak = true;
                                        break;
                                    }
                                }
                                if (isBreak)
                                {
                                    break;
                                }
                            }
                        }
                        else if (v is ReferredArea)
                        {
                            ReferredArea ra = (ReferredArea)v;
                            int rc = ra.EndRow - ra.StartRow + 1;
                            int cc = ra.EndColumn - ra.StartColumn + 1;
                            for (int r = 0; r &lt; rc; r++)
                            {
                                for (int c = 0; c &lt; cc; c++)
                                {
                                    object vi = ra.GetValue(r, c);
                                    if (IsBreak(vi))
                                    {
                                        isBreak = true;
                                        break;
                                    }
                                }
                                if (isBreak)
                                {
                                    break;
                                }
                            }
                        }
                        else
                        {
                            isBreak = IsBreak(v);
                        }
                        if (isBreak)
                        {
                            data.CalculatedValue = Indicator;
                            break;
                        }
                    }
                }
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


