---
title: Workbook.GetStyleInPool
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells
type: docs
url: /net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.

```csharp
public Style GetStyleInPool(int index)
```

| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |

### Return Value

The style in the pool corresponds to given index, may be null.

### Remarks

If the returned style is changed, the style of all cells(which refers to this style) will be changed.

### Examples

```csharp
// Called: style = wb.GetStyleInPool(i);
[Test]
        public void Method_Int32_()
        { //CELLSJAVA-41144
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style;
            for (int i = 0; i &lt; 8192; i++)
            {
                style = wb.CreateStyle();
                style.Name = &quot;testclean&quot; + i;
            }
            for (int i = 0; i &lt; 10; i++)
            {
                cell.SetStyle(wb.GetNamedStyle(&quot;testclean&quot; + i));
            }
            style = cell.GetStyle();
            style.Font.Color = Color.Red;
            cell.PutValue(&quot;Test cleanup stylepool, this cell&apos;s font color should be red.&quot;);
            cell.SetStyle(style);
            wb.RemoveUnusedStyles();
            wb.Save(new MemoryStream(), SaveFormat.Xlsx); //condense the pool
            AssertHelper.AreEqual(18, wb.CountOfStylesInPool, &quot;Styles in pool should be gathered and cleanup&quot;);
            int count = 0;
            for (int i = wb.CountOfStylesInPool - 1; i &gt; 15; i--)
            {
                style = wb.GetStyleInPool(i);
                if (style != null &amp;&amp; (style.Name == null || style.Name == &quot;&quot;))
                {
                    count++;
                }
            }
            AssertHelper.AreEqual(1, count, &quot;Styles in pool should be gathered and cleanup&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


