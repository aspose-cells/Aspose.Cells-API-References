---
title: Worksheet.ShowFormulas
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether to show formulas or their results
type: docs
url: /net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Indicates whether to show formulas or their results.

```csharp
public bool ShowFormulas { get; set; }
```

### Examples

```csharp
// Called: sheet2.ShowFormulas = false;
[Test]
        public void Property_ShowFormulas()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            double cw = cells.GetColumnWidth(0);
            int pw = cells.GetColumnWidthPixel(0);
            sheet.ShowFormulas = true;
            Assert.AreEqual(cw, cells.GetColumnWidth(0), 0.01, &quot;A-Width&quot;);
            Assert.AreEqual(pw*2, cells.GetColumnWidthPixel(0), &quot;A-WidthPixel&quot;);
            cells.SetColumnWidth(1, cw*2);
            Assert.AreEqual(cw*2, cells.GetColumnWidth(1), 0.01, &quot;B-Width after SetWidth&quot;);
            Assert.AreEqual(1.0, cells.GetColumnWidthPixel(1)/4.0/pw, 0.1, &quot;B-WidthPixel after SetWidth&quot;);
            cells.SetColumnWidthPixel(1, pw);
            Assert.AreEqual(1.0, cells.GetColumnWidth(1) * 2.0 / cw, 0.1, &quot;B-Width after SetWidthPixel&quot;);
            Assert.AreEqual(pw, cells.GetColumnWidthPixel(1), &quot;B-WidthPixel after SetWidthPixel&quot;);
            cells.SetColumnWidthPixel(2, pw * 2);
            Assert.AreEqual(cw, cells.GetColumnWidth(2), 0.01, &quot;C-Width after SetWidthPixel*2&quot;);
            Assert.AreEqual(pw * 2, cells.GetColumnWidthPixel(2), &quot;C-WidthPixel after SetWidthPixel*2&quot;);
            cells.SetColumnWidthPixel(3, pw * 4);
            Assert.AreEqual(1.0, cells.GetColumnWidth(3) / 2.0 / cw, 0.1, &quot;D-Width after SetWidthPixel*4&quot;);
            Assert.AreEqual(pw * 4, cells.GetColumnWidthPixel(3), &quot;D-WidthPixel after SetWidthPixel*4&quot;);
            Workbook wb2 = Util.ReSave(wb, SaveFormat.Xlsx);
            Worksheet sheet2 = wb.Worksheets[0];
            Cells cells2 = sheet.Cells;
            Assert.AreEqual(cw, cells2.GetColumnWidth(0), 0.01, &quot;A-Width2&quot;);
            Assert.AreEqual(pw * 2, cells2.GetColumnWidthPixel(0), &quot;A-WidthPixel2&quot;);
            Assert.AreEqual(1.0, cells.GetColumnWidth(1) * 2.0 / cw, 0.1, &quot;B-Widths&quot;);
            Assert.AreEqual(pw, cells.GetColumnWidthPixel(1), &quot;B-WidthPixel2&quot;);
            Assert.AreEqual(cw, cells.GetColumnWidth(2), 0.01, &quot;C-Width2&quot;);
            Assert.AreEqual(pw * 2, cells.GetColumnWidthPixel(2), &quot;C-WidthPixel2&quot;);
            Assert.AreEqual(1.0, cells.GetColumnWidth(3) / 2.0 / cw, 0.1, &quot;D-Width2&quot;);
            Assert.AreEqual(pw * 4, cells.GetColumnWidthPixel(3), &quot;D-WidthPixel2&quot;);
            sheet2.ShowFormulas = false;
            Assert.AreEqual(cw, cells2.GetColumnWidth(0), 0.01, &quot;A-Width2,NoShowFormula&quot;);
            Assert.AreEqual(pw, cells2.GetColumnWidthPixel(0), &quot;A-WidthPixel2,NoShowFormula&quot;);
            Assert.AreEqual(1.0, cells.GetColumnWidth(1) * 2.0 / cw, 0.1, &quot;B-Widths,NoShowFormula&quot;);
            Assert.AreEqual(pw/2, cells.GetColumnWidthPixel(1), &quot;B-WidthPixel2,NoShowFormula&quot;);
            Assert.AreEqual(cw, cells.GetColumnWidth(2), 0.01, &quot;C-Width2,NoShowFormula&quot;);
            Assert.AreEqual(pw, cells.GetColumnWidthPixel(2), &quot;C-WidthPixel2,NoShowFormula&quot;);
            Assert.AreEqual(1.0, cells.GetColumnWidth(3) / 2.0 / cw, 0.1, &quot;D-Width2,NoShowFormula&quot;);
            Assert.AreEqual(pw * 2, cells.GetColumnWidthPixel(3), &quot;D-WidthPixel2,NoShowFormula&quot;);
            //wb2.DefaultStyle.Font.Size = 20;
            //cells.CopyColumn(cells2, 1, 0); //does not use Column.Copy()
            //Assert.AreEqual(cells2.GetColumnWidthPixel(1)*2, cells.GetColumnWidthPixel(0), &quot;2.B-&gt;1.A&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


