---
title: Workbook.CreateBuiltinStyle
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Creates builtin style by given type
type: docs
url: /net/aspose.cells/workbook/createbuiltinstyle/
---
## Workbook.CreateBuiltinStyle method

Creates built-in style by given type.

```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | BuiltinStyleType | The builtin style stype. |

### Return Value

[`Style`](../../style/) object

### Examples

```csharp
// Called: Style style = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
public void Workbook_Method_CreateBuiltinStyle()
{
    Workbook workbook = new Workbook();


    workbook.Worksheets[0].Cells["A1"].PutValue("Good");

    Style style = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);

    workbook.Worksheets[0].Cells["A1"].SetStyle(style);
    Assert.AreEqual(style.ForegroundColor.ToArgb()&0xFFFFFF, 0xC6EFCE);


    workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");

    style = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);

    workbook.Worksheets[0].Cells["B2"].SetStyle(style);
    Assert.AreEqual(style.ForegroundColor.ToArgb() & 0xFFFFFF, 0xFFEB9C);

}
```

### See Also

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


