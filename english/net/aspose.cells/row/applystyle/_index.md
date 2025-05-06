---
title: Row.ApplyStyle
second_title: Aspose.Cells for .NET API Reference
description: Row method. Applies formats for a whole row
type: docs
url: /net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Applies formats for a whole row.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The style object which will be applied. |
| flag | StyleFlag | Flags which indicates applied formatting properties. |

### Examples

```csharp
// Called: cells.Rows[3].ApplyStyle(style, sf);
[Test]
        public void Method_StyleFlag_()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Style style = wb.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.CenterAcross;
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            cells.Columns[5].ApplyStyle(style, sf);
            cells.Columns[6].ApplyStyle(style, sf);
            cells.SetColumnWidth(5, 2);
            cells.SetColumnWidth(6, 2);
            cells.Rows[3].ApplyStyle(style, sf);
            style.HorizontalAlignment = TextAlignmentType.Right;
            cells.Rows[4].ApplyStyle(style, sf);
            style.HorizontalAlignment = TextAlignmentType.CenterAcross;
            for (int i = 0; i &lt; 5; i++)
            {
                cells[0, i].SetStyle(style);
                cells[1, i].SetStyle(style);
                cells[2, i].SetStyle(style);
                cells[4, i].SetStyle(style);
                cells.SetColumnWidth(i, 2);
            }
            int[] indices = new int[]
            {
                0x00, 0x10, 0x13, 0x20, 0x30, 0x33, 0x35, 0x40, 0x43,
            };
            foreach (int ci in indices)
            {
                cells[ci&gt;&gt;4, ci&amp;0x0F].PutValue(1.23456789);
            }
            cells.Merge(2, 0, 1, 3);
            style.HorizontalAlignment = TextAlignmentType.Right;
            cells[3, 9].SetStyle(style);

            string[] expected = new string[]
            { //in ms excel, 1.2346 should be 1.23457, D2 should be 1.23456789
                &quot;1.23456789&quot;, &quot;1.2346&quot;, &quot;1.234568&quot;,
                &quot;1.2346&quot;, &quot;1.2346&quot;, &quot;1.23&quot;,
                &quot;1.23456789&quot;, &quot;1.2346&quot;, &quot;1.23&quot;, 
            };
            StringBuilder sb = null;
            for (int i = 0; i &lt; indices.Length; i++)
            {
                string act = cells[indices[i] &gt;&gt; 4, indices[i] &amp; 0x0F].DisplayStringValue;
                if (!expected[i].Equals(act))
                {
                    if (sb == null)
                    {
                        sb = new StringBuilder();
                    }
                    sb.Append(CellsHelper.CellIndexToName(indices[i] &gt;&gt; 4, indices[i] &amp; 0x0F));
                    sb.Append(&quot;.DisplayStringValue expected &quot;);
                    sb.Append(expected[i]);
                    sb.Append(&quot; but was &quot;);
                    sb.Append(act);
                    sb.Append(&apos;\n&apos;);
                }
            }
            if (sb != null)
            {
                Assert.Fail(sb.ToString());
            }
        }
```

### See Also

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


