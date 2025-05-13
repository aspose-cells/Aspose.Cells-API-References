---
title: ReferredArea.StartRow
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The start row of the area
type: docs
url: /net/aspose.cells/referredarea/startrow/
---
## ReferredArea.StartRow property

The start row of the area.

```csharp
public int StartRow { get; }
```

### Examples

```csharp
// Called: int rc = ra.EndRow - ra.StartRow + 1;
public override void ReferredArea_Property_StartRow(CalculationData data)
            {
                if (data.FunctionName == "MYFUNC")
                {
                    data.CalculatedValue = Indicator;
                }
                else
                {
                    for (int i = data.ParamCount - 1; i > -1; i--)
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
                            for (int r = 0; r < rc; r++)
                            {
                                for (int c = 0; c < cc; c++)
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


