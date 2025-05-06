---
title: PivotArea.OnlyLabel
second_title: Aspose.Cells for .NET API Reference
description: PivotArea property. Indicates whether only the data labels for an item selection are selected
type: docs
url: /net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

Indicates whether only the data labels for an item selection are selected.

```csharp
public bool OnlyLabel { get; set; }
```

### Examples

```csharp
// Called: pt.PivotFormats[0].PivotArea.OnlyLabel = true;//onlydata = false
[Test]
        public void Property_OnlyLabel()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56640.xlsx&quot;);

            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;
            //onlydata is true, onlylabel = false
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(193, 229, 245), cells[&quot;G6&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(193, 229, 245), cells[&quot;G9&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G10&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G13&quot;].GetStyle().ForegroundColor));
            //G6 G9 G10 G13
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.PivotFormats[0].PivotArea.OnlyData = false;//onlylabel = false
            workbook.Worksheets.RefreshAll();
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G6&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G9&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G10&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G13&quot;].GetStyle().ForegroundColor));

            pt.PivotFormats[0].PivotArea.OnlyLabel = true;//onlydata = false
            workbook.Worksheets.RefreshAll();
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G6&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Red, cells[&quot;G9&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.Empty, cells[&quot;G10&quot;].GetStyle().ForegroundColor));
            Assert.IsTrue(Util.CompareColor(Color.FromArgb(193, 229, 245), cells[&quot;G13&quot;].GetStyle().ForegroundColor));
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET56640.html&quot;);
        }
```

### See Also

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


