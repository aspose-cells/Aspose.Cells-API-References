---
title: Style.Font
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets a Font object
type: docs
url: /net/aspose.cells/style/font/
---
## Style.Font property

Gets a `Font` object.

```csharp
public Font Font { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(s.Font.IsItalic, cn + &amp;quot;.FontItalic&amp;quot;);
[Test]
        public void Property_Font()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            Column column = cells.Columns[2];
            Style s = column.GetStyle();
            s.Pattern = BackgroundType.Solid;
            s.ForegroundColor = Color.Red;
            StyleFlag sf = new StyleFlag();
            sf.All = true;
            column.ApplyStyle(s, sf);
            column = cells.Columns[5];
            s.ForegroundColor = Color.Blue;
            column.ApplyStyle(s, sf);

            Cell cell = cells[3, 2];
            s.Pattern = BackgroundType.None;
            s.Font.IsItalic = true;
            cell.SetStyle(s);
            cell = cells[4, 2];
            cell.SetStyle(wb.CreateStyle());

            cell = cells[7, 1];
            cell.SetStyle(s);

            CellArea ca = CellArea.CreateCellArea(3, 3, 5, 5);
            cells.InsertRange(ca, ShiftType.Right);
            for (int j = ca.StartColumn; j &lt;= ca.EndColumn; j++)
            {
                s = cells[3, j].GetStyle();
                string cn = CellsHelper.CellIndexToName(3, j);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsTrue(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[4, j].GetStyle();
                cn = CellsHelper.CellIndexToName(4, j);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[5, j].GetStyle();
                cn = CellsHelper.CellIndexToName(5, j);
                Assert.AreEqual(BackgroundType.Solid, s.Pattern, cn + &quot;.Pattern&quot;);
                AssertHelper.AreEqual(Color.Red, s.ForegroundColor, cn + &quot;.ForeColor&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
            }
            for (int i = ca.StartRow; i &lt;= ca.EndRow; i++)
            {
                s = cells[i, 8].GetStyle();
                string cn = CellsHelper.CellIndexToName(i, 8);
                Assert.AreEqual(BackgroundType.Solid, s.Pattern, cn + &quot;.Pattern&quot;);
                AssertHelper.AreEqual(Color.Blue, s.ForegroundColor, cn + &quot;.ForeColor&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[i, 6].GetStyle();
                cn = CellsHelper.CellIndexToName(i, 6);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[i, 7].GetStyle();
                cn = CellsHelper.CellIndexToName(i, 7);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
            }

            ca = CellArea.CreateCellArea(7, 2, 9, 4);
            cells.InsertRange(ca, ShiftType.Right);
            for (int j = ca.StartColumn; j &lt;= ca.EndColumn; j++)
            {
                s = cells[7, j].GetStyle();
                string cn = CellsHelper.CellIndexToName(7, j);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsTrue(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[8, j].GetStyle();
                cn = CellsHelper.CellIndexToName(8, j);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
            }
            for (int i = ca.StartRow; i &lt;= ca.EndRow; i++)
            {
                s = cells[i, 5].GetStyle();
                string cn = CellsHelper.CellIndexToName(i, 5);
                Assert.AreEqual(BackgroundType.Solid, s.Pattern, cn + &quot;.Pattern&quot;);
                AssertHelper.AreEqual(Color.Red, s.ForegroundColor, cn + &quot;.ForeColor&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[i, 6].GetStyle();
                cn = CellsHelper.CellIndexToName(i, 6);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[i, 7].GetStyle();
                cn = CellsHelper.CellIndexToName(i, 7);
                Assert.AreEqual(BackgroundType.None, s.Pattern, cn + &quot;.Pattern&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
                s = cells[i, 8].GetStyle();
                cn = CellsHelper.CellIndexToName(i, 8);
                Assert.AreEqual(BackgroundType.Solid, s.Pattern, cn + &quot;.Pattern&quot;);
                AssertHelper.AreEqual(Color.Blue, s.ForegroundColor, cn + &quot;.ForeColor&quot;);
                Assert.IsFalse(s.Font.IsItalic, cn + &quot;.FontItalic&quot;);
            }
        }
```

### See Also

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


