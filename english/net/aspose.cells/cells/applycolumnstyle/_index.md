---
title: Cells.ApplyColumnStyle
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Applies formats for a whole column
type: docs
url: /net/aspose.cells/cells/applycolumnstyle/
---
## Cells.ApplyColumnStyle method

Applies formats for a whole column.

```csharp
public void ApplyColumnStyle(int column, Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | The column index. |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: cells.ApplyColumnStyle(1, style, flag);
[Test]
        public void Method_StyleFlag_()
        {
            object[,] data = new object[2, 2] { { &quot;07/14/14&quot;, &quot;1.234&quot; }, { &quot;1.2E3&quot;, &quot;01/02/15 10:20&quot; } };
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            Style style = cell.GetStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            cell.SetStyle(style);
            StyleFlag flag = new StyleFlag();
            flag.All = true;
            cells.ApplyColumnStyle(1, style, flag);
            cells.ApplyRowStyle(1, style, flag);
            cells.ImportTwoDimensionArray(data, null, 0, 0, new TxtLoadOptions(LoadFormat.Csv)
            {
                ConvertDateTimeData = true,
                ConvertNumericData = true,
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn,
            });
            Check43298Style(&quot;A1&quot;, cell.GetStyle(), 14, &quot;&quot;);
            Check43298Style(&quot;B1&quot;, cells[0, 1].GetStyle(), 0, &quot;&quot;);
            Check43298Style(&quot;A2&quot;, cells[1, 0].GetStyle(), 0, &quot;#.#E+0&quot;);
            Check43298Style(&quot;B2&quot;, cells[1, 1].GetStyle(), 22, &quot;&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


