---
title: Workbook.RemoveUnusedStyles
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Remove all unused styles
type: docs
url: /net/aspose.cells/workbook/removeunusedstyles/
---
## Workbook.RemoveUnusedStyles method

Remove all unused styles.

```csharp
public void RemoveUnusedStyles()
```

### Examples

```csharp
// Called: wb.RemoveUnusedStyles();
[Test]
        public void Method_RemoveUnusedStyles()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            int count = wb.CountOfStylesInPool;
            int pos = 16;
            for (; pos &lt; count; pos++)
            {
                if (wb.GetStyleInPool(pos) == null)
                {
                    break;
                }
            }
            Style style = cell.GetStyle();
            style.Font.Color = Color.Red;
            cell.SetStyle(style);
            AssertHelper.AreEqual(Color.Red, wb.GetStyleInPool(pos).Font.Color, &quot;Cell style&apos;s index in pool should be &quot; + pos);
            int pos1 = pos;
            pos++;
            if (pos &gt; count)
            {
                count++;
            }
            else
            {
                for (; pos &lt; count; pos++)
                {
                    if (wb.GetStyleInPool(pos) == null)
                    {
                        break;
                    }
                }
            }
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;After setting cell&apos;s style, style count&quot;);

            style.Font.Color = Color.Gray;
            cell.SetStyle(style);
            AssertHelper.AreEqual(Color.Gray, wb.GetStyleInPool(pos).Font.Color, &quot;First changing cell&apos;s style, cell style&apos;s index in pool should be &quot; + pos);
            if (pos == count)
            {
                count++;
            }
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;After change cell&apos;s style, style count&quot;);
            wb.RemoveUnusedStyles();
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;Removing unused style should not change style count in pool&quot;);
            Assert.AreEqual(null, wb.GetStyleInPool(pos1), &quot;Removing unused style should make the previous cell style at &quot; + pos1 + &quot; empty&quot;);
            pos1 = pos;
            pos = 16;
            for (; pos &lt; count; pos++)
            {
                if (wb.GetStyleInPool(pos) == null)
                {
                    break;
                }
            }
            style.Font.Color = Color.Yellow;
            cell.SetStyle(style);
            AssertHelper.AreEqual(Color.Yellow, wb.GetStyleInPool(pos).Font.Color, &quot;Reuse item in pool, cell style&apos;s index in pool should be &quot; + pos);
            if (pos == count)
            {
                count++;
            }
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;Second changing cell&apos;s style, style count should be&quot;);
            for (pos = count - 1; pos &gt; 15; pos--)
            {
                if (wb.GetStyleInPool(pos) == null || pos == pos1)
                {
                    count--;
                }
                else
                {
                    break;
                }
            }
            wb.RemoveUnusedStyles();
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;Second changing cell&apos;s style, style count&quot;);
            if (pos1 &lt; count)
            {
                Assert.AreEqual(null, wb.GetStyleInPool(pos1), &quot;Second removing unused style should make the previous cell style at &quot; + (pos1) + &quot; empty&quot;);
            }

            style.Name = &quot;TestNamedStyle&quot;;
            count++;
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;After adding NamedStyle, style count&quot;);
            cell.SetStyle(style);
            count++;
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;After adding cell style referencing to NamedStyle, style count&quot;);
            wb.RemoveUnusedStyles();
            wb.Save(new MemoryStream(), SaveFormat.Xlsx);
            count--;
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;After adding cell style referencing to NamedStyle, style count&quot;);
            //CELLSNET-46840: removing and saving again cause the NamedStyle being removed
            wb.RemoveUnusedStyles();
            wb.Save(new MemoryStream(), SaveFormat.Xlsx);
            Assert.AreEqual(count, wb.CountOfStylesInPool, &quot;After adding cell style referencing to NamedStyle, style count&quot;);

            wb = new Workbook(Constants.sourcePath + &quot;Copy/copy_001.xls&quot;);
            cells = wb.Worksheets[0].Cells;
            Workbook wb1 = new Workbook(Constants.sourcePath + &quot;Copy/testAlignmentSetting.xls&quot;);
            Cells cells1 = wb1.Worksheets[0].Cells;
            cells.CopyRows(cells1, 0, 1, 30);
            count = wb.CountOfStylesInPool;
            wb.RemoveUnusedStyles();
            wb = Util.ReSave(wb, SaveFormat.Excel97To2003);
            Assert.IsTrue(count &gt; wb.CountOfStylesInPool, &quot;The resaved workbook1&apos;s style count should less than the copied resultant.&quot;);

            wb = new Workbook(Constants.sourcePath + &quot;Copy/copy_001.xls&quot;);
            cells = wb.Worksheets[0].Cells;
            cells1.CopyColumns(cells, 0, 1, 30);
            count = wb1.CountOfStylesInPool;
            wb1.RemoveUnusedStyles();
            wb1 = Util.ReSave(wb1, SaveFormat.Excel97To2003);
            Assert.IsTrue(count &gt; wb1.CountOfStylesInPool, &quot;The resaved workbook2&apos;s style count should less than the copied resultant.&quot;);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


