---
title: Column.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Column method. Applies formats for a whole column
type: docs
url: /net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Applies formats for a whole column.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: c.ApplyStyle(s, sf);
[Test]
        public void Method_StyleFlag_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 8].Value = &quot;End&quot;;
            Column c = cells.Columns[1];
            Style s = wb.CreateStyle();
            s.Pattern = BackgroundType.Solid;
            s.ForegroundColor = Color.Red;
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            c.ApplyStyle(s, sf);
            Aspose.Cells.Range r1 = cells.CreateRange(0, 0, 1, 3);
            Aspose.Cells.Range r2 = cells.CreateRange(0, 4, 1, 3);
            r2.Copy(r1);
            s = cells[0, 5].GetStyle();
            Assert.AreEqual(BackgroundType.Solid, s.Pattern, &quot;Pattern&quot;);
            AssertHelper.AreEqual(Color.Red, s.ForegroundColor, &quot;Color&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


