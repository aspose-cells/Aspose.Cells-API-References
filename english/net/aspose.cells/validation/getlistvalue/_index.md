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
// Called: object v = vldt.GetListValue(i, 2);
public void Validation_Method_GetListValue()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Validation vldt = wb.Worksheets[0].Cells["C9"].GetValidation();
    string[] expected = new string[]
    {
        null, "Sheet3!$G$5:$G$110", "Sheet3!$G$31:$G$110", "Sheet3!$G$26:$G$110", "Sheet3!$G$2:$G$110",
        "Sheet3!$G$91:$G$110", "Sheet3!$G$32:$G$110", "Sheet3!$G$54:$G$110", "Sheet3!$G$75:$G$110",
        "Sheet3!$G$36:$G$110", "Sheet3!$G$109:$G$110", "Sheet3!$G$18:$G$110", "Sheet3!$G$30:$G$110", null
    };
    for (int i = 6; i < 20; i++)
    {
        object v = vldt.GetListValue(i, 2);
        Assert.AreEqual(expected[i - 6], v == null ? null : ((ReferredArea)v).ToString(), "C" + (i + 1));
    }
    vldt.Formula1 = "abc,def";
    for (int i = 7; i < 18; i++)
    {
        object[] v = (object[])vldt.GetListValue(i, 2);
        Assert.AreEqual("abc", v[0], "C" + (i + 1) + ".[0]");
        Assert.AreEqual("def", v[1], "C" + (i + 1) + ".[1]");
    }
    vldt.Formula1 = "abc";
    for (int i = 7; i < 18; i++)
    {
        object v = vldt.GetListValue(i, 2);
        Assert.AreEqual("abc", v, "C" + (i + 1));
    }
}
```

### See Also

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


