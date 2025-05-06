---
title: ReferredArea.GetValue
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea method. Gets cell value with given offset from the topleft of this area
type: docs
url: /net/aspose.cells/referredarea/getvalue/
---
## GetValue(int, int) {#getvalue}

Gets cell value with given offset from the top-left of this area.

```csharp
public object GetValue(int rowOffset, int colOffset)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | row offset from the start row of this area |
| colOffset | Int32 | column offset from the start row of this area |

### Return Value

"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### Examples

```csharp
// Called: double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
public override void Method_Int32_(CalculationData data)
        {
            // Example: Custom implementation for a function named &quot;MYFUNC&quot;
            if (data.FunctionName.ToUpper() == &quot;MYFUNC&quot;)
            {
                // Assuming MYFUNC takes two parameters and returns their sum
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValue(int, int, bool) {#getvalue_1}

Gets cell value with given offset from the top-left of this area.

```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | row offset from the start row of this area |
| colOffset | Int32 | column offset from the start row of this area |
| calculateFormulas | Boolean | Whether calculate it recursively if the specified reference is formula |

### Return Value

"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.

### Examples

```csharp
// Called: data.CalculatedValue = ra.GetValue(0, 0, true);
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


