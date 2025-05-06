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
[Test]
        public void Method_BuiltinStyleType_()
        {
            Workbook workbook = new Workbook();


            workbook.Worksheets[0].Cells[&quot;A1&quot;].PutValue(&quot;Good&quot;);

            Style style = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);

            workbook.Worksheets[0].Cells[&quot;A1&quot;].SetStyle(style);
            Assert.AreEqual(style.ForegroundColor.ToArgb()&amp;0xFFFFFF, 0xC6EFCE);


            workbook.Worksheets[0].Cells[&quot;B2&quot;].PutValue(&quot;Neutral&quot;);

            style = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);

            workbook.Worksheets[0].Cells[&quot;B2&quot;].SetStyle(style);
            Assert.AreEqual(style.ForegroundColor.ToArgb() &amp; 0xFFFFFF, 0xFFEB9C);

        }
```

### See Also

* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


