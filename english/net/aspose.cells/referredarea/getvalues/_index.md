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
// Called: calculated = ((ReferredArea)calculated).GetValues();
public static void Method_GetValues(string fml, double expected, double delta, Worksheet sheet, string msg)
        {
            object calculated = sheet.CalculateFormula(fml);
            if (calculated is ReferredArea)
            {
                calculated = ((ReferredArea)calculated).GetValues();
            }
            if (calculated is int)
            {
                if (IsEqual(expected, (int)calculated, delta))
                {
                    return;
                }
            }
            else if (calculated is double)
            {
                if (IsEqual(expected, (double)calculated, delta))
                {
                    return;
                }
            }
            Assert.Fail(fml + &quot;: Required numeric value &quot; + expected + &quot; but was &quot; + calculated);
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
public override void Method_Boolean_(CalculationData data)
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


