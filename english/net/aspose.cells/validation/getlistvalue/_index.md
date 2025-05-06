---
title: Validation.GetListValue
second_title: Aspose.Cells for .NET API Reference
description: Validation method. Get the value for list of the validation for the specified cell
type: docs
url: /net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

Get the value for list of the validation for the specified cell.

```csharp
public object GetListValue(int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |

### Return Value

The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a [`ReferredArea`](../../referredarea/) object; Otherwise the returned value may be null, object[], or simple object.

### Remarks

Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.

### Examples

```csharp
// Called: object[] v = (object[])vldt.GetListValue(i, 2);
[Test]
        public void Method_Int32_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Validation/J42738.xlsx&quot;);
            Validation vldt = wb.Worksheets[0].Cells[&quot;C9&quot;].GetValidation();
            string[] expected = new string[]
            {
                null, &quot;Sheet3!$G$5:$G$110&quot;, &quot;Sheet3!$G$31:$G$110&quot;, &quot;Sheet3!$G$26:$G$110&quot;, &quot;Sheet3!$G$2:$G$110&quot;,
                &quot;Sheet3!$G$91:$G$110&quot;, &quot;Sheet3!$G$32:$G$110&quot;, &quot;Sheet3!$G$54:$G$110&quot;, &quot;Sheet3!$G$75:$G$110&quot;,
                &quot;Sheet3!$G$36:$G$110&quot;, &quot;Sheet3!$G$109:$G$110&quot;, &quot;Sheet3!$G$18:$G$110&quot;, &quot;Sheet3!$G$30:$G$110&quot;, null
            };
            for (int i = 6; i &lt; 20; i++)
            {
                object v = vldt.GetListValue(i, 2);
                Assert.AreEqual(expected[i - 6], v == null ? null : ((ReferredArea)v).ToString(), &quot;C&quot; + (i + 1));
            }
            vldt.Formula1 = &quot;abc,def&quot;;
            for (int i = 7; i &lt; 18; i++)
            {
                object[] v = (object[])vldt.GetListValue(i, 2);
                Assert.AreEqual(&quot;abc&quot;, v[0], &quot;C&quot; + (i + 1) + &quot;.[0]&quot;);
                Assert.AreEqual(&quot;def&quot;, v[1], &quot;C&quot; + (i + 1) + &quot;.[1]&quot;);
            }
            vldt.Formula1 = &quot;abc&quot;;
            for (int i = 7; i &lt; 18; i++)
            {
                object v = vldt.GetListValue(i, 2);
                Assert.AreEqual(&quot;abc&quot;, v, &quot;C&quot; + (i + 1));
            }
        }
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


