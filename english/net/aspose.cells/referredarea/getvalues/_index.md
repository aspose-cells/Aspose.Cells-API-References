---
title: ReferredArea.GetValues
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea method. Gets cell values in this area
type: docs
url: /net/aspose.cells/referredarea/getvalues/
---
## GetValues() {#getvalues}

Gets cell values in this area.

```csharp
public object GetValues()
```

### Return Value

If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### Examples

```csharp
// Called: object vs = ra.GetValues();
private void ReferredArea_Method_GetValues(ReferredArea ra)
            {
                object vs = ra.GetValues();
                if (vs is Array)
                {
                    object[][] avs = (object[][])vs;
                    foreach (object[] rd in avs)
                    {
                        foreach (object v in rd)
                        {
                            Console.WriteLine(_copts == null ? "default:" + v : "norecursive: " + v);
                        }
                    }
                }
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValues(bool) {#getvalues_1}

Gets cell values in this area.

```csharp
public object GetValues(bool calculateFormulas)
```

| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | Boolean | In this range, if there are some formulas that have not been calculated, this flag denotes whether those formulas should be calculated recursively |

### Return Value

If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

### Examples

```csharp
// Called: object res = ra.GetValues(false);
public override void ReferredArea_Method_GetValues(CalculationData data)
            {
                if (_inProcess)
                {
                    data.CalculatedValue = -_type;
                    return;
                }
                _inProcess = true;
                ReferredArea ra = (ReferredArea) data.GetParamValue(0);
                switch (_type)
                {
                    case 1:
                    {
                        object res = ra.GetValues();
                        data.CalculatedValue = res is object[] ? ((object[]) res)[0] : res;
                        break;
                    }
                    case 2:
                    {
                        object res = ra.GetValues(true);
                        data.CalculatedValue = res is object[] ? ((object[])res)[0] : res;
                        break;
                    }
                    case 3:
                    {
                        object res = ra.GetValues(false);
                        data.CalculatedValue = res is object[] ? ((object[])res)[0] : res;
                        break;
                    }
                    case 4:
                    {
                        data.CalculatedValue = ra.GetValue(0, 0);
                        break;
                    }
                    case 5:
                    {
                        data.CalculatedValue = ra.GetValue(0, 0, true);
                        break;
                    }
                    case 6:
                    {
                        data.CalculatedValue = ra.GetValue(0, 0, false);
                        break;
                    }
                }
                _inProcess = false;
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


