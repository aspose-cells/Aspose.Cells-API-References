---
title: Range.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Range method. Applies formats for a whole range
type: docs
url: /net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Applies formats for a whole range.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Remarks

Each cell in this range will contains a [`Style`](../../style/) object. So this is a memory-consuming method. Please use it carefully.

### Examples

```csharp
// Called: area.ApplyStyle(style, new StyleFlag() { All = true });
[Test]
        public void Method_StyleFlag_()
        {

            Workbook wb = new Workbook(Constants.sourcePath + &quot;AsposeStyle.xlsx&quot;);
            var workhsheet = wb.Worksheets[0];
            var style = wb.GetNamedStyle(&quot;TestStyle1&quot;);
            workhsheet.Cells[0, 0].SetStyle(style);


            Aspose.Cells.Range area = workhsheet.Cells.CreateRange(0, 2, 1, 1);
            area.ApplyStyle(style, new StyleFlag() { All = true });
            style = workhsheet.Cells[0, 0].GetStyle();
            Assert.AreEqual(workhsheet.Cells[0, 0].StringValue, &quot;$12,345.00&quot;);
            Assert.AreEqual(style.Pattern, BackgroundType.None);
            style = workhsheet.Cells[0, 2].GetStyle();
            Assert.AreEqual(style.Pattern, BackgroundType.None);

                
            wb.Save(Constants.destPath + &quot;AsposeStyle.xlsx&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


