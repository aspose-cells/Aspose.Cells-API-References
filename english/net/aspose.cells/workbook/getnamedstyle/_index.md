---
title: Workbook.GetNamedStyle
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets the named style in the style pool
type: docs
url: /net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Gets the named style in the style pool.

```csharp
public Style GetNamedStyle(string name)
```

| Parameter | Type | Description |
| --- | --- | --- |
| name | String | name of the style |

### Return Value

named style, maybe null.

### Examples

```csharp
// Called: Assert.IsTrue(workbook.GetNamedStyle(&amp;quot;Style 1&amp;quot;) != null);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CustomNamedStyle.xlsx&quot;);
            Assert.IsTrue(workbook.GetNamedStyle(&quot;Style 1&quot;) != null);
        }
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


